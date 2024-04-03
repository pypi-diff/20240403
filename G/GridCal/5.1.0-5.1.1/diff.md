# Comparing `tmp/GridCal-5.1.0.tar.gz` & `tmp/GridCal-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GridCal-5.1.0.tar", last modified: Mon Apr  1 07:49:43 2024, max compression
+gzip compressed data, was "GridCal-5.1.1.tar", last modified: Wed Apr  3 10:11:21 2024, max compression
```

## Comparing `GridCal-5.1.0.tar` & `GridCal-5.1.1.tar`

### file list

```diff
@@ -1,260 +1,264 @@
--rw-rw-r--   0 santi     (1000) santi     (1000)     2808 2024-04-01 07:49:22.778443 GridCal-5.1.0/GridCal/__version__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      654 2023-11-16 09:36:26.514645 GridCal-5.1.0/GridCal/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1545 2024-03-11 19:28:12.151075 GridCal-5.1.0/GridCal/ExecuteGridCal.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11713 2024-03-11 19:28:12.175075 GridCal-5.1.0/GridCal/LICENSE.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)     2965 2024-01-05 08:44:35.533288 GridCal-5.1.0/GridCal/update.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5188 2024-03-11 19:28:12.175075 GridCal-5.1.0/GridCal/templates.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8747 2024-03-28 10:16:48.968877 GridCal-5.1.0/GridCal/Session/results_model.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4257 2024-03-14 19:48:07.680505 GridCal-5.1.0/GridCal/Session/export_results_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21120 2024-03-14 19:48:07.680505 GridCal-5.1.0/GridCal/Session/session.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13285 2024-03-14 19:48:07.680505 GridCal-5.1.0/GridCal/Session/synchronization_driver.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-14 19:48:07.680505 GridCal-5.1.0/GridCal/Session/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6822 2024-03-14 19:48:07.680505 GridCal-5.1.0/GridCal/Session/file_handler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33193 2022-08-17 15:43:33.049797 GridCal-5.1.0/GridCal/data/cables.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2022-08-17 15:43:33.033797 GridCal-5.1.0/GridCal/data/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      376 2023-11-16 09:36:26.518645 GridCal-5.1.0/GridCal/data/sequence_lines.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)    55648 2023-11-16 09:36:26.518645 GridCal-5.1.0/GridCal/data/transformers.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)     5013 2022-08-17 15:43:33.045797 GridCal-5.1.0/GridCal/data/wires.csv
--rw-rw-r--   0 santi     (1000) santi     (1000)    25703 2024-03-14 19:48:07.672505 GridCal-5.1.0/GridCal/Gui/GeneralDialogues.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1634 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/update_gui_all.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.0/GridCal/Gui/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2551 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/messages.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2969 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/themes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3978 2024-02-13 14:28:28.563734 GridCal-5.1.0/GridCal/Gui/ConsoleWidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    85018 2024-03-28 10:16:48.956877 GridCal-5.1.0/GridCal/Gui/GuiFunctions.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/plot_config.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3740 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/update_gui_common.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.0/GridCal/Gui/Widgets/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7365 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/Widgets/matplotlibwidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45061 2023-11-16 09:36:26.514645 GridCal-5.1.0/GridCal/Gui/Widgets/custom_qrangeslider.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.0/GridCal/Gui/ContingencyPlanner/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.0/GridCal/Gui/ContingencyPlanner/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15460 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/ContingencyPlanner/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5241 2024-03-11 19:28:12.159075 GridCal-5.1.0/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11953 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/ContingencyPlanner/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.0/GridCal/Gui/CoordinatesInput/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.0/GridCal/Gui/CoordinatesInput/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    39352 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/CoordinatesInput/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9471 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/CoordinatesInput/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15110 2024-03-11 19:28:12.159075 GridCal-5.1.0/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.0/GridCal/Gui/TowerBuilder/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.0/GridCal/Gui/TowerBuilder/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11704 2024-03-11 19:28:12.175075 GridCal-5.1.0/GridCal/Gui/TowerBuilder/table_models.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4789 2023-11-16 09:36:26.506645 GridCal-5.1.0/GridCal/Gui/TowerBuilder/test_.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21426 2024-03-14 19:48:07.680505 GridCal-5.1.0/GridCal/Gui/TowerBuilder/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16061 2024-03-14 19:48:07.680505 GridCal-5.1.0/GridCal/Gui/TowerBuilder/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11180 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.082158 GridCal-5.1.0/GridCal/Gui/BusViewer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.0/GridCal/Gui/BusViewer/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    25810 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/BusViewer/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6537 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/BusViewer/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10406 2024-03-11 19:28:12.159075 GridCal-5.1.0/GridCal/Gui/BusViewer/bus_viewer_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7262 2024-03-11 19:28:12.151075 GridCal-5.1.0/GridCal/Gui/AboutDialogue/about_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.082158 GridCal-5.1.0/GridCal/Gui/AboutDialogue/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.082158 GridCal-5.1.0/GridCal/Gui/AboutDialogue/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14879 2024-02-29 08:22:37.932355 GridCal-5.1.0/GridCal/Gui/AboutDialogue/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11275 2024-03-11 19:28:12.151075 GridCal-5.1.0/GridCal/Gui/AboutDialogue/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/ProfilesInput/excel_dialog.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      243 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/ProfilesInput/profiles_from_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/ProfilesInput/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    16317 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      353 2023-06-09 13:30:46.098158 GridCal-5.1.0/GridCal/Gui/ProfilesInput/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11691 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/ProfilesInput/models_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    45917 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/ProfilesInput/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24295 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/ProfilesInput/profile_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5707 2023-11-16 09:36:26.502645 GridCal-5.1.0/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2420 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/ProfilesInput/excel_sheet_selection.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/Analysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      485 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/Analysis/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    21495 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/Analysis/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3871 2024-03-11 19:28:12.151075 GridCal-5.1.0/GridCal/Gui/Analysis/AnalysisDialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18860 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/Analysis/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    48733 2024-04-01 07:29:23.256927 GridCal-5.1.0/GridCal/Gui/Analysis/object_plot_analysis.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5003 2024-03-11 19:28:12.159075 GridCal-5.1.0/GridCal/Gui/CascadingSteps/cascading_steps.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/CascadingSteps/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      281 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/CascadingSteps/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5684 2023-11-16 09:36:26.482645 GridCal-5.1.0/GridCal/Gui/CascadingSteps/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1464 2024-02-13 14:28:28.563734 GridCal-5.1.0/GridCal/Gui/Main/ConsoleLogController.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4843 2024-03-28 10:16:48.956877 GridCal-5.1.0/GridCal/Gui/Main/GridCalMain.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   272576 2024-04-01 07:49:22.774443 GridCal-5.1.0/GridCal/Gui/Main/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.0/GridCal/Gui/Main/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      591 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/Main/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5157 2024-04-01 07:38:27.483690 GridCal-5.1.0/GridCal/Gui/Main/ConsoleLog.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   769321 2024-04-01 07:49:22.778443 GridCal-5.1.0/GridCal/Gui/Main/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2195 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/Main/object_select_window.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      359 2023-11-16 09:36:26.490645 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/README.txt
--rw-rw-r--   0 santi     (1000) santi     (1000)   109995 2024-03-28 10:16:48.960877 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/simulations.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    33619 2024-03-28 10:16:48.960877 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/io.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31214 2024-03-14 19:48:07.676505 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/base_gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3784 2024-02-13 14:28:28.567734 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Scripting/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5813 2024-04-01 07:49:22.774443 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Scripting/scripting.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Settings/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14965 2024-03-28 10:16:48.960877 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Settings/configuration.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    44200 2024-03-28 10:16:48.960877 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Model/objects.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    20949 2024-03-28 10:16:48.960877 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Model/time_events.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Model/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    72302 2024-03-28 10:16:48.956877 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Model/diagrams.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5891 2024-03-11 19:28:12.163075 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Results/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12771 2024-03-14 19:48:07.676505 GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Results/results.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.0/GridCal/Gui/Visualization/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2838 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/Visualization/visualization.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11934 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/Visualization/palettes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6843 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    53448 2024-03-14 19:48:07.680505 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/node_breaker_editor_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2918 2024-03-28 10:16:48.968877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/generic_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/matplotlibwidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5185 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/terminal_item.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7549 2024-03-28 10:16:48.964877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Fluid/fluid_turbine_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7093 2024-03-28 10:16:48.964877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Fluid/fluid_pump_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Fluid/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9879 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Fluid/fluid_path_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7083 2024-03-28 10:16:48.964877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Fluid/fluid_p2x_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14515 2024-03-28 10:16:48.964877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Fluid/fluid_node_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4713 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/winding_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13983 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4191 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/switch_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 12:16:24.348976 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    12042 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/dc_line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4357 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/hvdc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4304 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/upfc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9137 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/transformer2w_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8824 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/line_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4505 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/vsc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10040 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/transformer_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14166 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/Rectangle_Connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30235 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/line_graphics_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7357 2024-03-28 10:16:48.968877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/static_generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6209 2024-03-28 10:16:48.968877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/injections_template_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6903 2024-03-28 10:16:48.964877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/battery_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7749 2024-03-28 10:16:48.968877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/shunt_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7349 2024-03-28 10:16:48.964877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/external_grid_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6520 2024-03-28 10:16:48.968877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/load_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19553 2024-03-28 10:16:48.968877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Substation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    25814 2024-03-28 10:16:48.968877 GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Substation/bus_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.0/GridCal/Gui/SyncDialogue/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.0/GridCal/Gui/SyncDialogue/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14939 2023-11-16 09:36:26.506645 GridCal-5.1.0/GridCal/Gui/SyncDialogue/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3233 2024-03-14 19:48:07.680505 GridCal-5.1.0/GridCal/Gui/SyncDialogue/sync_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4684 2023-11-16 09:36:26.506645 GridCal-5.1.0/GridCal/Gui/SyncDialogue/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6556 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.0/GridCal/Gui/SolarPowerWizard/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.506645 GridCal-5.1.0/GridCal/Gui/SolarPowerWizard/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18492 2023-11-16 09:36:26.506645 GridCal-5.1.0/GridCal/Gui/SolarPowerWizard/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7914 2023-11-16 09:36:26.506645 GridCal-5.1.0/GridCal/Gui/SolarPowerWizard/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   160053 2024-03-28 10:16:48.964877 GridCal-5.1.0/GridCal/Gui/MapWidget/map_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5067 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/MapWidget/node_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2418 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/map_events.py
--rw-rw-r--   0 santi     (1000) santi     (1000)       36 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/logger.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18838 2024-03-28 10:16:48.964877 GridCal-5.1.0/GridCal/Gui/MapWidget/grid_map_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3351 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/tile_worker.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13789 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/tiles.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6092 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/base_tiles.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2757 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/tiles_cache.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2974 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/pycacheback.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30307 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/default_tile_data.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4856 2024-03-28 10:16:48.964877 GridCal-5.1.0/GridCal/Gui/MapWidget/Schema/Nodes.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2081 2024-03-28 10:16:48.964877 GridCal-5.1.0/GridCal/Gui/MapWidget/Schema/Connector.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-01 07:37:07.951895 GridCal-5.1.0/GridCal/Gui/MapWidget/Schema/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1836 2024-03-28 10:16:48.964877 GridCal-5.1.0/GridCal/Gui/MapWidget/Schema/SchemaManager.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      121 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/layer_types.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3628 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/point_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3902 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/image_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      282 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/place.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3633 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/polyline_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3882 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/text_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3739 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/polygon_layer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2933 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/open_street_map.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2340 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/mapbox.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2895 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/cartodb.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2504 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/mapquest.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2592 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/stamen_transport.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2410 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/stamen_watercolor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2382 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/blue_marble.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2399 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/stamen_toner.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4265 2023-11-16 09:36:26.498645 GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/gmt_local.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    24893 2023-11-16 09:36:26.502645 GridCal-5.1.0/GridCal/Gui/RosetaExplorer/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.0/GridCal/Gui/RosetaExplorer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.502645 GridCal-5.1.0/GridCal/Gui/RosetaExplorer/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    18469 2024-03-11 19:28:12.171075 GridCal-5.1.0/GridCal/Gui/RosetaExplorer/RosetaExplorer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1976 2023-11-16 09:36:26.502645 GridCal-5.1.0/GridCal/Gui/RosetaExplorer/ConsoleWidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   225320 2023-11-16 09:36:26.502645 GridCal-5.1.0/GridCal/Gui/RosetaExplorer/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.486645 GridCal-5.1.0/GridCal/Gui/LoadDesigner/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.689061 GridCal-5.1.0/GridCal/Gui/LoadDesigner/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5615 2024-03-17 11:12:27.689061 GridCal-5.1.0/GridCal/Gui/LoadDesigner/load_designer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.689061 GridCal-5.1.0/GridCal/Gui/LoadDesigner/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13073 2024-03-17 11:12:27.689061 GridCal-5.1.0/GridCal/Gui/LoadDesigner/load_designer_ui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-02-13 14:28:28.571734 GridCal-5.1.0/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.0/GridCal/Gui/WindPowerWizard/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.514645 GridCal-5.1.0/GridCal/Gui/WindPowerWizard/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9724 2023-11-16 09:36:26.514645 GridCal-5.1.0/GridCal/Gui/WindPowerWizard/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7869 2023-11-16 09:36:26.514645 GridCal-5.1.0/GridCal/Gui/WindPowerWizard/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 11:12:27.693060 GridCal-5.1.0/GridCal/Gui/SystemScaler/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.693060 GridCal-5.1.0/GridCal/Gui/SystemScaler/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9718 2024-03-28 10:16:48.968877 GridCal-5.1.0/GridCal/Gui/SystemScaler/system_scaler.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.693060 GridCal-5.1.0/GridCal/Gui/SystemScaler/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4357 2024-03-17 11:12:27.693060 GridCal-5.1.0/GridCal/Gui/SystemScaler/system_scaler_ui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4262 2023-11-16 09:36:26.506645 GridCal-5.1.0/GridCal/Gui/TreeModelViewer/MainWindow.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.0/GridCal/Gui/TreeModelViewer/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.514645 GridCal-5.1.0/GridCal/Gui/TreeModelViewer/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   224984 2023-11-16 09:36:26.514645 GridCal-5.1.0/GridCal/Gui/TreeModelViewer/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8686 2024-03-11 19:28:12.175075 GridCal-5.1.0/GridCal/Gui/TreeModelViewer/TreeModelViewer.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      914 2024-02-13 14:28:28.563734 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     2918 2024-03-28 10:16:48.956877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/generic_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-02-13 14:28:28.563734 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/matplotlibwidget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8059 2024-03-28 16:37:46.596741 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/terminal_item.py
--rw-rw-r--   0 santi     (1000) santi     (1000)   182587 2024-04-01 07:29:23.256927 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/bus_branch_editor_widget.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6531 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Fluid/fluid_turbine_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6076 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Fluid/fluid_pump_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.559734 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Fluid/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6099 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Fluid/fluid_path_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6065 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Fluid/fluid_p2x_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    17393 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Fluid/fluid_node_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4486 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/winding_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    13080 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     3961 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/switch_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 12:13:24.384980 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4087 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/series_reactance_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    11846 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/dc_line_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4404 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/hvdc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4042 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/upfc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     8966 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/transformer2w_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     9431 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/line_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4242 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/vsc_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    14035 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/transformer3w_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    10044 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/transformer_editor.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    31115 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/line_graphics_template.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6439 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/static_generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.563734 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6408 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/current_injection_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6402 2024-04-01 07:29:23.256927 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/injections_template_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5969 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/battery_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6481 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/shunt_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6434 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/external_grid_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     6402 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/controllable_shunt_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5683 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/load_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    19255 2024-03-28 10:16:48.952877 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/generator_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-02-13 14:28:28.563734 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Substation/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    30848 2024-03-28 16:37:48.632741 GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Substation/bus_graphics.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.0/GridCal/Gui/SigmaAnalysis/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.102158 GridCal-5.1.0/GridCal/Gui/SigmaAnalysis/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    41704 2023-11-16 09:36:26.502645 GridCal-5.1.0/GridCal/Gui/SigmaAnalysis/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4758 2023-11-16 09:36:26.502645 GridCal-5.1.0/GridCal/Gui/SigmaAnalysis/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4018 2024-03-14 19:48:07.680505 GridCal-5.1.0/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.0/GridCal/Gui/GridGenerator/__init__.py
--rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.090158 GridCal-5.1.0/GridCal/Gui/GridGenerator/update_gui_file.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     5329 2024-03-11 19:28:12.159075 GridCal-5.1.0/GridCal/Gui/GridGenerator/grid_generator_dialogue.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15613 2023-11-16 09:36:26.486645 GridCal-5.1.0/GridCal/Gui/GridGenerator/icons_rc.py
--rw-rw-r--   0 santi     (1000) santi     (1000)    15239 2023-11-16 09:36:26.486645 GridCal-5.1.0/GridCal/Gui/GridGenerator/gui.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     4902 2024-03-11 19:28:12.175075 GridCal-5.1.0/setup.py
--rw-rw-r--   0 santi     (1000) santi     (1000)     1043 2024-04-01 07:49:43.030409 GridCal-5.1.0/PKG-INFO
--rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-01 07:49:43.030409 GridCal-5.1.0/setup.cfg
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2808 2024-04-03 10:10:53.840547 GridCal-5.1.1/GridCal/__version__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      654 2023-11-16 09:36:26.514645 GridCal-5.1.1/GridCal/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1545 2024-03-11 19:28:12.151075 GridCal-5.1.1/GridCal/ExecuteGridCal.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11713 2024-03-11 19:28:12.175075 GridCal-5.1.1/GridCal/LICENSE.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2965 2024-01-05 08:44:35.533288 GridCal-5.1.1/GridCal/update.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5188 2024-03-11 19:28:12.175075 GridCal-5.1.1/GridCal/templates.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8747 2024-03-28 10:16:48.968877 GridCal-5.1.1/GridCal/Session/results_model.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4257 2024-03-14 19:48:07.680505 GridCal-5.1.1/GridCal/Session/export_results_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21120 2024-03-14 19:48:07.680505 GridCal-5.1.1/GridCal/Session/session.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13285 2024-03-14 19:48:07.680505 GridCal-5.1.1/GridCal/Session/synchronization_driver.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-14 19:48:07.680505 GridCal-5.1.1/GridCal/Session/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6822 2024-03-14 19:48:07.680505 GridCal-5.1.1/GridCal/Session/file_handler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33193 2022-08-17 15:43:33.049797 GridCal-5.1.1/GridCal/data/cables.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2022-08-17 15:43:33.033797 GridCal-5.1.1/GridCal/data/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      376 2023-11-16 09:36:26.518645 GridCal-5.1.1/GridCal/data/sequence_lines.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)    55648 2023-11-16 09:36:26.518645 GridCal-5.1.1/GridCal/data/transformers.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5013 2022-08-17 15:43:33.045797 GridCal-5.1.1/GridCal/data/wires.csv
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25703 2024-03-14 19:48:07.672505 GridCal-5.1.1/GridCal/Gui/GeneralDialogues.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1634 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/update_gui_all.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.1/GridCal/Gui/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2551 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/messages.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2969 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/themes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3978 2024-02-13 14:28:28.563734 GridCal-5.1.1/GridCal/Gui/ConsoleWidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    85090 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/GuiFunctions.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1986 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/plot_config.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3740 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/update_gui_common.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.1/GridCal/Gui/Widgets/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7365 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/Widgets/matplotlibwidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45061 2023-11-16 09:36:26.514645 GridCal-5.1.1/GridCal/Gui/Widgets/custom_qrangeslider.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.1/GridCal/Gui/ContingencyPlanner/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.1/GridCal/Gui/ContingencyPlanner/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15460 2023-11-16 09:36:26.482645 GridCal-5.1.1/GridCal/Gui/ContingencyPlanner/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5241 2024-03-11 19:28:12.159075 GridCal-5.1.1/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11953 2023-11-16 09:36:26.482645 GridCal-5.1.1/GridCal/Gui/ContingencyPlanner/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.1/GridCal/Gui/CoordinatesInput/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.086158 GridCal-5.1.1/GridCal/Gui/CoordinatesInput/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    39352 2023-11-16 09:36:26.482645 GridCal-5.1.1/GridCal/Gui/CoordinatesInput/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9471 2023-11-16 09:36:26.482645 GridCal-5.1.1/GridCal/Gui/CoordinatesInput/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15110 2024-03-11 19:28:12.159075 GridCal-5.1.1/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.1/GridCal/Gui/TowerBuilder/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.1/GridCal/Gui/TowerBuilder/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11704 2024-03-11 19:28:12.175075 GridCal-5.1.1/GridCal/Gui/TowerBuilder/table_models.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4789 2023-11-16 09:36:26.506645 GridCal-5.1.1/GridCal/Gui/TowerBuilder/test_.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21426 2024-03-14 19:48:07.680505 GridCal-5.1.1/GridCal/Gui/TowerBuilder/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16061 2024-03-14 19:48:07.680505 GridCal-5.1.1/GridCal/Gui/TowerBuilder/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11180 2024-03-11 19:28:12.171075 GridCal-5.1.1/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6235 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/graphics_manager.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusViewer/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusViewer/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25810 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusViewer/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6537 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusViewer/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10449 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusViewer/bus_viewer_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6818 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    53583 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/node_breaker_editor_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2918 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/generic_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/matplotlibwidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5194 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/terminal_item.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7576 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Fluid/fluid_turbine_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7120 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Fluid/fluid_pump_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Fluid/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9924 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Fluid/fluid_path_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7110 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Fluid/fluid_p2x_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14569 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Fluid/fluid_node_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4740 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/winding_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14019 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4191 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/switch_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12069 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/dc_line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4384 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/hvdc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4331 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/upfc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9173 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/transformer2w_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8824 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/line_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4532 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/vsc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10040 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/transformer_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14211 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/Rectangle_Connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30271 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/line_graphics_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7384 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/static_generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6227 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/injections_template_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6930 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/battery_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7776 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/shunt_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7376 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/external_grid_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6556 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/load_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19589 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Substation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    25895 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Substation/bus_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   160152 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/map_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5067 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/node_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2418 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/map_events.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)       36 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/logger.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18974 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3360 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13730 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6101 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2766 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2974 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30307 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4856 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2090 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Schema/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1854 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      121 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/layer_types.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3646 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3920 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      282 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/place.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3651 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3900 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3757 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2942 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2349 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2904 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2513 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2601 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2419 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2391 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2408 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4274 2024-04-03 10:10:53.828547 GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      792 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6776 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/generic_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7801 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/matplotlibwidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8113 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/terminal_item.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   178435 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/bus_branch_editor_widget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6421 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Fluid/fluid_turbine_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6103 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Fluid/fluid_pump_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Fluid/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6120 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Fluid/fluid_path_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6092 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Fluid/fluid_p2x_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    17563 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Fluid/fluid_node_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4478 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/winding_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13081 2024-04-03 10:10:53.820547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3978 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/switch_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.820547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4104 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/series_reactance_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11838 2024-04-03 10:10:53.820547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/dc_line_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4396 2024-04-03 10:10:53.820547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/hvdc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4059 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/upfc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9001 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/transformer2w_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9431 2024-04-03 10:10:53.820547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/line_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4259 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/vsc_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14071 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/transformer3w_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    10044 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/transformer_editor.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30372 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/line_graphics_template.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6416 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/static_generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6435 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/current_injection_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5949 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/injections_template_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5996 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/battery_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6508 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/shunt_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6436 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/external_grid_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6429 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/controllable_shunt_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5648 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/load_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    19291 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/generator_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Substation/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30204 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Substation/busbar_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30225 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Substation/cn_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    30201 2024-04-03 10:10:53.824547 GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Substation/bus_graphics.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7262 2024-03-11 19:28:12.151075 GridCal-5.1.1/GridCal/Gui/AboutDialogue/about_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.082158 GridCal-5.1.1/GridCal/Gui/AboutDialogue/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.082158 GridCal-5.1.1/GridCal/Gui/AboutDialogue/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14879 2024-02-29 08:22:37.932355 GridCal-5.1.1/GridCal/Gui/AboutDialogue/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11275 2024-03-11 19:28:12.151075 GridCal-5.1.1/GridCal/Gui/AboutDialogue/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1217 2023-11-16 09:36:26.498645 GridCal-5.1.1/GridCal/Gui/ProfilesInput/excel_dialog.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      243 2023-11-16 09:36:26.498645 GridCal-5.1.1/GridCal/Gui/ProfilesInput/profiles_from_data.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.498645 GridCal-5.1.1/GridCal/Gui/ProfilesInput/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    16317 2023-11-16 09:36:26.498645 GridCal-5.1.1/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      353 2023-06-09 13:30:46.098158 GridCal-5.1.1/GridCal/Gui/ProfilesInput/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11691 2024-03-11 19:28:12.171075 GridCal-5.1.1/GridCal/Gui/ProfilesInput/models_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    45917 2023-11-16 09:36:26.498645 GridCal-5.1.1/GridCal/Gui/ProfilesInput/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24295 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/ProfilesInput/profile_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5707 2023-11-16 09:36:26.502645 GridCal-5.1.1/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2420 2023-11-16 09:36:26.498645 GridCal-5.1.1/GridCal/Gui/ProfilesInput/excel_sheet_selection.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.1/GridCal/Gui/Analysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      485 2023-11-16 09:36:26.482645 GridCal-5.1.1/GridCal/Gui/Analysis/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    21495 2023-11-16 09:36:26.482645 GridCal-5.1.1/GridCal/Gui/Analysis/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3871 2024-03-11 19:28:12.151075 GridCal-5.1.1/GridCal/Gui/Analysis/AnalysisDialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18860 2023-11-16 09:36:26.482645 GridCal-5.1.1/GridCal/Gui/Analysis/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    48733 2024-04-01 07:29:23.256927 GridCal-5.1.1/GridCal/Gui/Analysis/object_plot_analysis.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5003 2024-03-11 19:28:12.159075 GridCal-5.1.1/GridCal/Gui/CascadingSteps/cascading_steps.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.482645 GridCal-5.1.1/GridCal/Gui/CascadingSteps/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      281 2023-11-16 09:36:26.482645 GridCal-5.1.1/GridCal/Gui/CascadingSteps/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5684 2023-11-16 09:36:26.482645 GridCal-5.1.1/GridCal/Gui/CascadingSteps/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1464 2024-02-13 14:28:28.563734 GridCal-5.1.1/GridCal/Gui/Main/ConsoleLogController.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4843 2024-03-28 10:16:48.956877 GridCal-5.1.1/GridCal/Gui/Main/GridCalMain.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   272769 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Main/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.1/GridCal/Gui/Main/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      591 2023-11-16 09:36:26.498645 GridCal-5.1.1/GridCal/Gui/Main/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5157 2024-04-03 08:20:19.176693 GridCal-5.1.1/GridCal/Gui/Main/ConsoleLog.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   776230 2024-04-03 10:10:53.840547 GridCal-5.1.1/GridCal/Gui/Main/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2195 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/Main/object_select_window.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      359 2023-11-16 09:36:26.490645 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/README.txt
+-rw-rw-r--   0 santi     (1000) santi     (1000)   110029 2024-04-03 10:10:53.836547 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/simulations.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    33653 2024-04-03 10:10:53.836547 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/io.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    31223 2024-04-03 10:10:53.836547 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/base_gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3784 2024-02-13 14:28:28.567734 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Scripting/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5813 2024-04-01 07:49:22.774443 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Scripting/scripting.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Settings/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15008 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Settings/configuration.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    44209 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Model/objects.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    20949 2024-03-28 10:16:48.960877 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Model/time_events.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Model/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    72324 2024-04-03 10:10:53.832547 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Model/diagrams.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5891 2024-03-11 19:28:12.163075 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.490645 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Results/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    12771 2024-03-14 19:48:07.676505 GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Results/results.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.1/GridCal/Gui/Visualization/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     2838 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/Visualization/visualization.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    11934 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/Visualization/palettes.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.102158 GridCal-5.1.1/GridCal/Gui/SyncDialogue/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      303 2023-06-09 13:30:46.102158 GridCal-5.1.1/GridCal/Gui/SyncDialogue/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    14939 2023-11-16 09:36:26.506645 GridCal-5.1.1/GridCal/Gui/SyncDialogue/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3233 2024-03-14 19:48:07.680505 GridCal-5.1.1/GridCal/Gui/SyncDialogue/sync_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4684 2023-11-16 09:36:26.506645 GridCal-5.1.1/GridCal/Gui/SyncDialogue/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     6556 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.1/GridCal/Gui/SolarPowerWizard/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.506645 GridCal-5.1.1/GridCal/Gui/SolarPowerWizard/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18492 2023-11-16 09:36:26.506645 GridCal-5.1.1/GridCal/Gui/SolarPowerWizard/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7914 2023-11-16 09:36:26.506645 GridCal-5.1.1/GridCal/Gui/SolarPowerWizard/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    24893 2023-11-16 09:36:26.502645 GridCal-5.1.1/GridCal/Gui/RosetaExplorer/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.1/GridCal/Gui/RosetaExplorer/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.502645 GridCal-5.1.1/GridCal/Gui/RosetaExplorer/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    18469 2024-03-11 19:28:12.171075 GridCal-5.1.1/GridCal/Gui/RosetaExplorer/RosetaExplorer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1976 2023-11-16 09:36:26.502645 GridCal-5.1.1/GridCal/Gui/RosetaExplorer/ConsoleWidget.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   225320 2023-11-16 09:36:26.502645 GridCal-5.1.1/GridCal/Gui/RosetaExplorer/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.486645 GridCal-5.1.1/GridCal/Gui/LoadDesigner/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.689061 GridCal-5.1.1/GridCal/Gui/LoadDesigner/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5615 2024-03-17 11:12:27.689061 GridCal-5.1.1/GridCal/Gui/LoadDesigner/load_designer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.689061 GridCal-5.1.1/GridCal/Gui/LoadDesigner/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    13073 2024-03-17 11:12:27.689061 GridCal-5.1.1/GridCal/Gui/LoadDesigner/load_designer_ui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     3692 2024-02-13 14:28:28.571734 GridCal-5.1.1/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.514645 GridCal-5.1.1/GridCal/Gui/WindPowerWizard/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-11-16 09:36:26.514645 GridCal-5.1.1/GridCal/Gui/WindPowerWizard/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9724 2023-11-16 09:36:26.514645 GridCal-5.1.1/GridCal/Gui/WindPowerWizard/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     7869 2023-11-16 09:36:26.514645 GridCal-5.1.1/GridCal/Gui/WindPowerWizard/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2024-03-17 11:12:27.693060 GridCal-5.1.1/GridCal/Gui/SystemScaler/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      316 2024-03-17 11:12:27.693060 GridCal-5.1.1/GridCal/Gui/SystemScaler/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     9718 2024-03-28 10:16:48.968877 GridCal-5.1.1/GridCal/Gui/SystemScaler/system_scaler.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    37622 2024-03-17 11:12:27.693060 GridCal-5.1.1/GridCal/Gui/SystemScaler/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4357 2024-03-17 11:12:27.693060 GridCal-5.1.1/GridCal/Gui/SystemScaler/system_scaler_ui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4262 2023-11-16 09:36:26.506645 GridCal-5.1.1/GridCal/Gui/TreeModelViewer/MainWindow.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.506645 GridCal-5.1.1/GridCal/Gui/TreeModelViewer/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      574 2023-11-16 09:36:26.514645 GridCal-5.1.1/GridCal/Gui/TreeModelViewer/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)   224984 2023-11-16 09:36:26.514645 GridCal-5.1.1/GridCal/Gui/TreeModelViewer/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     8686 2024-03-11 19:28:12.175075 GridCal-5.1.1/GridCal/Gui/TreeModelViewer/TreeModelViewer.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-11-16 09:36:26.502645 GridCal-5.1.1/GridCal/Gui/SigmaAnalysis/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.102158 GridCal-5.1.1/GridCal/Gui/SigmaAnalysis/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    41704 2023-11-16 09:36:26.502645 GridCal-5.1.1/GridCal/Gui/SigmaAnalysis/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4758 2023-11-16 09:36:26.502645 GridCal-5.1.1/GridCal/Gui/SigmaAnalysis/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4018 2024-03-14 19:48:07.680505 GridCal-5.1.1/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)        0 2023-06-09 13:30:46.086158 GridCal-5.1.1/GridCal/Gui/GridGenerator/__init__.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)      302 2023-06-09 13:30:46.090158 GridCal-5.1.1/GridCal/Gui/GridGenerator/update_gui_file.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     5329 2024-03-11 19:28:12.159075 GridCal-5.1.1/GridCal/Gui/GridGenerator/grid_generator_dialogue.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15613 2023-11-16 09:36:26.486645 GridCal-5.1.1/GridCal/Gui/GridGenerator/icons_rc.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)    15239 2023-11-16 09:36:26.486645 GridCal-5.1.1/GridCal/Gui/GridGenerator/gui.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     4902 2024-03-11 19:28:12.175075 GridCal-5.1.1/setup.py
+-rw-rw-r--   0 santi     (1000) santi     (1000)     1043 2024-04-03 10:11:21.536547 GridCal-5.1.1/PKG-INFO
+-rw-rw-r--   0 santi     (1000) santi     (1000)       37 2024-04-03 10:11:21.536547 GridCal-5.1.1/setup.cfg
```

### Comparing `GridCal-5.1.0/GridCal/__version__.py` & `GridCal-5.1.1/GridCal/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with GridCal.  If not, see <http://www.gnu.org/licenses/>.
 import datetime
 _current_year_ = datetime.datetime.now().year
 
 # do not forget to keep a three-number version!!!
-__GridCal_VERSION__ = "5.1.0"
+__GridCal_VERSION__ = "5.1.1"
 
 url = 'https://github.com/SanPen/GridCal'
 
 about_msg = "GridCal v" + str(__GridCal_VERSION__) + '\n\n'
 
 about_msg += """
 GridCal has been carefully crafted since 2015 to
```

### Comparing `GridCal-5.1.0/GridCal/__init__.py` & `GridCal-5.1.1/GridCal/__init__.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/ExecuteGridCal.py` & `GridCal-5.1.1/GridCal/ExecuteGridCal.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/LICENSE.txt` & `GridCal-5.1.1/GridCal/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/update.py` & `GridCal-5.1.1/GridCal/update.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/templates.py` & `GridCal-5.1.1/GridCal/templates.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Session/results_model.py` & `GridCal-5.1.1/GridCal/Session/results_model.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Session/export_results_driver.py` & `GridCal-5.1.1/GridCal/Session/export_results_driver.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Session/session.py` & `GridCal-5.1.1/GridCal/Session/session.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Session/synchronization_driver.py` & `GridCal-5.1.1/GridCal/Session/synchronization_driver.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Session/file_handler.py` & `GridCal-5.1.1/GridCal/Session/file_handler.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/data/cables.csv` & `GridCal-5.1.1/GridCal/data/cables.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/data/transformers.csv` & `GridCal-5.1.1/GridCal/data/transformers.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/data/wires.csv` & `GridCal-5.1.1/GridCal/data/wires.csv`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/GeneralDialogues.py` & `GridCal-5.1.1/GridCal/Gui/GeneralDialogues.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/update_gui_all.py` & `GridCal-5.1.1/GridCal/Gui/update_gui_all.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/messages.py` & `GridCal-5.1.1/GridCal/Gui/messages.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/themes.py` & `GridCal-5.1.1/GridCal/Gui/themes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/ConsoleWidget.py` & `GridCal-5.1.1/GridCal/Gui/ConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/GuiFunctions.py` & `GridCal-5.1.1/GridCal/Gui/GuiFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 from GridCalEngine.basic_structures import IntVec
 from GridCalEngine.data_logger import DataLogger
 from GridCalEngine.IO.cim.cgmes.cgmes_circuit import CgmesCircuit, IdentifiedObject
 from GridCalEngine.Devices.Branches.line_locations import LineLocations
 from GridCalEngine.Devices.types import ALL_DEV_TYPES
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
-    from GridCal.Gui.MapWidget.grid_map_widget import GridMapWidget
-    from GridCal.Gui.BusViewer.bus_viewer_dialogue import BusViewerWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.MapWidget.grid_map_widget import GridMapWidget
+    from GridCal.Gui.Diagrams.BusViewer.bus_viewer_dialogue import BusViewerWidget
 
 
 class TreeDelegate(QtWidgets.QItemDelegate):
     """
     A delegate that places a fully functioning QComboBox in every
     cell of the column to which it's applied
     """
@@ -2355,17 +2355,17 @@
 
             self.update()
 
 
 class DiagramsModel(QtCore.QAbstractListModel):
     """
     Model for the diagrams
-    # from GridCal.Gui.BusViewer.bus_viewer_dialogue import BusViewerGUI
+    # from GridCal.Gui.Diagrams.BusViewer.bus_viewer_dialogue import BusViewerGUI
     # from GridCal.Gui.BusBranchEditorWidget import BusBranchEditorWidget
-    # from GridCal.Gui.MapWidget.grid_map_widget import GridMapWidget
+    # from GridCal.Gui.Diagrams.MapWidget.grid_map_widget import GridMapWidget
     """
 
     def __init__(self, list_of_diagrams: List[Union[BusBranchEditorWidget, GridMapWidget, BusViewerWidget]]):
         """
         Enumeration model
         :param list_of_diagrams: list of enumeration values to show
         """
@@ -2411,17 +2411,17 @@
             diagram = self.items[index.row()]
 
             if role == QtCore.Qt.ItemDataRole.DisplayRole:
                 return diagram.name
             elif role == QtCore.Qt.ItemDataRole.DecorationRole:
 
                 # TODO: Is this the only way?
-                from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
-                from GridCal.Gui.MapWidget.grid_map_widget import GridMapWidget
-                from GridCal.Gui.BusViewer.bus_viewer_dialogue import BusViewerWidget
+                from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+                from GridCal.Gui.Diagrams.MapWidget.grid_map_widget import GridMapWidget
+                from GridCal.Gui.Diagrams.BusViewer.bus_viewer_dialogue import BusViewerWidget
 
                 if isinstance(diagram, BusBranchEditorWidget):
                     return self.bus_branch_editor_icon
                 elif isinstance(diagram, GridMapWidget):
                     return self.map_editor_icon
                 elif isinstance(diagram, BusViewerWidget):
                     return self.bus_branch_vecinity_icon
```

### Comparing `GridCal-5.1.0/GridCal/Gui/plot_config.py` & `GridCal-5.1.1/GridCal/Gui/plot_config.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/update_gui_common.py` & `GridCal-5.1.1/GridCal/Gui/update_gui_common.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Widgets/matplotlibwidget.py` & `GridCal-5.1.1/GridCal/Gui/Widgets/matplotlibwidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Widgets/custom_qrangeslider.py` & `GridCal-5.1.1/GridCal/Gui/Widgets/custom_qrangeslider.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/ContingencyPlanner/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/ContingencyPlanner/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py` & `GridCal-5.1.1/GridCal/Gui/ContingencyPlanner/contingency_planner_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/ContingencyPlanner/gui.py` & `GridCal-5.1.1/GridCal/Gui/ContingencyPlanner/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/CoordinatesInput/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/CoordinatesInput/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/CoordinatesInput/gui.py` & `GridCal-5.1.1/GridCal/Gui/CoordinatesInput/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py` & `GridCal-5.1.1/GridCal/Gui/CoordinatesInput/coordinates_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/TowerBuilder/table_models.py` & `GridCal-5.1.1/GridCal/Gui/TowerBuilder/table_models.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/TowerBuilder/test_.py` & `GridCal-5.1.1/GridCal/Gui/TowerBuilder/test_.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/TowerBuilder/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/TowerBuilder/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/TowerBuilder/gui.py` & `GridCal-5.1.1/GridCal/Gui/TowerBuilder/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py` & `GridCal-5.1.1/GridCal/Gui/TowerBuilder/LineBuilderDialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/BusViewer/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusViewer/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/BusViewer/gui.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusViewer/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/BusViewer/bus_viewer_dialogue.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusViewer/bus_viewer_dialogue.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 import sys
 from PySide6 import QtWidgets
 
 from typing import List, Union
-from GridCal.Gui.BusViewer.gui import Ui_BusViewerWindow, QMainWindow
-from GridCal.Gui.BusBranchEditorWidget import BusBranchEditorWidget, generate_bus_branch_diagram
+from GridCal.Gui.Diagrams.BusViewer.gui import Ui_BusViewerWindow, QMainWindow
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget, generate_bus_branch_diagram
 import GridCalEngine.Devices as dev
 from GridCalEngine.enumerations import DeviceType
 from GridCalEngine.Devices.multi_circuit import MultiCircuit
 from GridCalEngine.Devices.Substation import Bus
 
 
 class BusViewerWidget(QMainWindow):
```

### Comparing `GridCal-5.1.0/GridCal/Gui/AboutDialogue/about_dialogue.py` & `GridCal-5.1.1/GridCal/Gui/AboutDialogue/about_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/AboutDialogue/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/AboutDialogue/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/AboutDialogue/gui.py` & `GridCal-5.1.1/GridCal/Gui/AboutDialogue/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/ProfilesInput/excel_dialog.py` & `GridCal-5.1.1/GridCal/Gui/ProfilesInput/excel_dialog.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py` & `GridCal-5.1.1/GridCal/Gui/ProfilesInput/profiles_from_data_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/ProfilesInput/models_dialogue.py` & `GridCal-5.1.1/GridCal/Gui/ProfilesInput/models_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/ProfilesInput/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/ProfilesInput/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/ProfilesInput/profile_dialogue.py` & `GridCal-5.1.1/GridCal/Gui/ProfilesInput/profile_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py` & `GridCal-5.1.1/GridCal/Gui/ProfilesInput/profiles_from_models_gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/ProfilesInput/excel_sheet_selection.py` & `GridCal-5.1.1/GridCal/Gui/ProfilesInput/excel_sheet_selection.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Analysis/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/Analysis/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Analysis/AnalysisDialogue.py` & `GridCal-5.1.1/GridCal/Gui/Analysis/AnalysisDialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Analysis/gui.py` & `GridCal-5.1.1/GridCal/Gui/Analysis/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Analysis/object_plot_analysis.py` & `GridCal-5.1.1/GridCal/Gui/Analysis/object_plot_analysis.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/CascadingSteps/cascading_steps.py` & `GridCal-5.1.1/GridCal/Gui/CascadingSteps/cascading_steps.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/CascadingSteps/gui.py` & `GridCal-5.1.1/GridCal/Gui/CascadingSteps/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/ConsoleLogController.py` & `GridCal-5.1.1/GridCal/Gui/Main/ConsoleLogController.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/GridCalMain.py` & `GridCal-5.1.1/GridCal/Gui/Main/GridCalMain.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/MainWindow.py` & `GridCal-5.1.1/GridCal/Gui/Main/MainWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -4553,14 +4553,17 @@
         self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_7), QCoreApplication.translate("mainWindow", u"Tables", None))
 #if QT_CONFIG(tooltip)
         self.saveResultsLogsButton.setToolTip(QCoreApplication.translate("mainWindow", u"Save the logs to a file", None))
 #endif // QT_CONFIG(tooltip)
         self.saveResultsLogsButton.setText("")
         self.tabWidget_4.setTabText(self.tabWidget_4.indexOf(self.tab_14), QCoreApplication.translate("mainWindow", u"Logs", None))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.ResultsTab), QCoreApplication.translate("mainWindow", u"Results", None))
+#if QT_CONFIG(tooltip)
+        self.clearSourceCodeButton.setToolTip(QCoreApplication.translate("mainWindow", u"New script, will delete the existing code.", None))
+#endif // QT_CONFIG(tooltip)
         self.clearSourceCodeButton.setText("")
 #if QT_CONFIG(tooltip)
         self.saveSourceCodeButton.setToolTip(QCoreApplication.translate("mainWindow", u"Save the current source code", None))
 #endif // QT_CONFIG(tooltip)
         self.saveSourceCodeButton.setText("")
 #if QT_CONFIG(tooltip)
         self.sourceCodeNameLineEdit.setToolTip(QCoreApplication.translate("mainWindow", u"Name of the source code file", None))
```

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/update_gui_file.py` & `GridCal-5.1.1/GridCal/Gui/Main/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/ConsoleLog.py` & `GridCal-5.1.1/GridCal/Gui/Main/ConsoleLog.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/Main/icons_rc.py`

 * *Files 1% similar despite different names*

```diff
@@ -11775,14 +11775,206 @@
 0076\x22\x0a       x=\x22\
 12.352184\x22\x0a     \
   id=\x22tspan885\x22\x0a\
        sodipodi:\
 role=\x22line\x22>~</t\
 span></text>\x0a</s\
 vg>\x0a\
+\x00\x00\x0b\xdf\
+<\
+?xml version=\x221.\
+0\x22 encoding=\x22UTF\
+-8\x22 standalone=\x22\
+no\x22?>\x0a<svg\x0a   wi\
+dth=\x2248\x22\x0a   heig\
+ht=\x2248\x22\x0a   viewB\
+ox=\x220 0 48 48\x22\x0a \
+  version=\x221.1\x22\x0a\
+   id=\x22svg4\x22\x0a   \
+sodipodi:docname\
+=\x22bus_bar_icon.s\
+vg\x22\x0a   inkscape:\
+version=\x221.1.2 (\
+0a00cf5339, 2022\
+-02-04)\x22\x0a   xmln\
+s:inkscape=\x22http\
+://www.inkscape.\
+org/namespaces/i\
+nkscape\x22\x0a   xmln\
+s:sodipodi=\x22http\
+://sodipodi.sour\
+ceforge.net/DTD/\
+sodipodi-0.dtd\x22\x0a\
+   xmlns=\x22http:/\
+/www.w3.org/2000\
+/svg\x22\x0a   xmlns:s\
+vg=\x22http://www.w\
+3.org/2000/svg\x22\x0a\
+   xmlns:rdf=\x22ht\
+tp://www.w3.org/\
+1999/02/22-rdf-s\
+yntax-ns#\x22\x0a   xm\
+lns:cc=\x22http://c\
+reativecommons.o\
+rg/ns#\x22\x0a   xmlns\
+:dc=\x22http://purl\
+.org/dc/elements\
+/1.1/\x22>\x0a  <metad\
+ata\x0a     id=\x22met\
+adata10\x22>\x0a    <r\
+df:RDF>\x0a      <c\
+c:Work\x0a         \
+rdf:about=\x22\x22>\x0a  \
+      <dc:format\
+>image/svg+xml</\
+dc:format>\x0a     \
+   <dc:type\x0a    \
+       rdf:resou\
+rce=\x22http://purl\
+.org/dc/dcmitype\
+/StillImage\x22 />\x0a\
+      </cc:Work>\
+\x0a    </rdf:RDF>\x0a\
+  </metadata>\x0a  \
+<defs\x0a     id=\x22d\
+efs8\x22 />\x0a  <sodi\
+podi:namedview\x0a \
+    pagecolor=\x22#\
+ffffff\x22\x0a     bor\
+dercolor=\x22#66666\
+6\x22\x0a     borderop\
+acity=\x221\x22\x0a     o\
+bjecttolerance=\x22\
+10\x22\x0a     gridtol\
+erance=\x2210\x22\x0a    \
+ guidetolerance=\
+\x2210\x22\x0a     inksca\
+pe:pageopacity=\x22\
+0\x22\x0a     inkscape\
+:pageshadow=\x222\x22\x0a\
+     inkscape:wi\
+ndow-width=\x222505\
+\x22\x0a     inkscape:\
+window-height=\x221\
+016\x22\x0a     id=\x22na\
+medview6\x22\x0a     s\
+howgrid=\x22false\x22\x0a\
+     inkscape:zo\
+om=\x224.2760417\x22\x0a \
+    inkscape:cx=\
+\x220.70158343\x22\x0a   \
+  inkscape:cy=\x229\
+3.193666\x22\x0a     i\
+nkscape:window-x\
+=\x2255\x22\x0a     inksc\
+ape:window-y=\x2227\
+\x22\x0a     inkscape:\
+window-maximized\
+=\x221\x22\x0a     inksca\
+pe:current-layer\
+=\x22svg4\x22\x0a     ink\
+scape:pagechecke\
+rboard=\x220\x22 />\x0a  \
+<g\x0a     id=\x22g845\
+\x22\x0a     transform\
+=\x22translate(0.88\
+479263,-4.423963\
+1)\x22\x0a     style=\x22\
+fill:#333333;str\
+oke:#333333\x22>\x0a  \
+  <rect\x0a       r\
+y=\x220\x22\x0a       y=\x22\
+21.161293\x22\x0a     \
+  x=\x225.0138187\x22\x0a\
+       height=\x227\
+.0783424\x22\x0a      \
+ width=\x227.373271\
+9\x22\x0a       id=\x22re\
+ct835\x22\x0a       st\
+yle=\x22opacity:0.8\
+53;fill:#333333;\
+fill-opacity:1;s\
+troke:#333333;st\
+roke-width:0.014\
+24989;stroke-lin\
+ecap:square;stro\
+ke-linejoin:beve\
+l;stroke-miterli\
+mit:4;stroke-das\
+harray:none;stro\
+ke-dashoffset:0;\
+stroke-opacity:1\
+;paint-order:str\
+oke fill markers\
+\x22 />\x0a    <path\x0a \
+      inkscape:c\
+onnector-curvatu\
+re=\x220\x22\x0a       id\
+=\x22path816\x22\x0a     \
+  d=\x22M 7.4185002\
+,35.023041 H 40.\
+655232\x22\x0a       s\
+tyle=\x22fill:#3333\
+33;fill-rule:eve\
+nodd;stroke:#333\
+333;stroke-width\
+:6.43819857;stro\
+ke-linecap:round\
+;stroke-linejoin\
+:miter;stroke-mi\
+terlimit:4;strok\
+e-dasharray:none\
+;stroke-opacity:\
+1\x22 />\x0a    <text\x0a\
+       id=\x22text8\
+39\x22\x0a       y=\x2228\
+.373415\x22\x0a       \
+x=\x2215.050968\x22\x0a  \
+     style=\x22font\
+-style:normal;fo\
+nt-variant:norma\
+l;font-weight:no\
+rmal;font-stretc\
+h:normal;font-si\
+ze:7.91466px;lin\
+e-height:125%;fo\
+nt-family:'Alte \
+Haas Grotesk';-i\
+nkscape-font-spe\
+cification:'Alte\
+ Haas Grotesk';l\
+etter-spacing:0p\
+x;word-spacing:0\
+px;fill:#333333;\
+fill-opacity:1;s\
+troke:#333333;st\
+roke-width:0.197\
+867px;stroke-lin\
+ecap:butt;stroke\
+-linejoin:miter;\
+stroke-opacity:1\
+\x22\x0a       xml:spa\
+ce=\x22preserve\x22\x0a  \
+     transform=\x22\
+scale(1.022082,0\
+.97839505)\x22><tsp\
+an\x0a         styl\
+e=\x22fill:#333333;\
+fill-opacity:1;s\
+troke:#333333;st\
+roke-width:0.197\
+867px\x22\x0a         \
+y=\x2228.373415\x22\x0a  \
+       x=\x2215.050\
+968\x22\x0a         id\
+=\x22tspan837\x22\x0a    \
+     sodipodi:ro\
+le=\x22line\x22>BusBar\
+</tspan></text>\x0a\
+  </g>\x0a</svg>\x0a\
 \x00\x00\x09\xe9\
 <\
 ?xml version=\x221.\
 0\x22 encoding=\x22UTF\
 -8\x22 standalone=\x22\
 no\x22?>\x0a<!-- Creat\
 ed with Inkscape\
@@ -20029,14 +20221,127 @@
 round;stroke-lin\
 ejoin:round;stro\
 ke-miterlimit:4;\
 stroke-dasharray\
 :none;stroke-opa\
 city:1\x22 />\x0a</svg\
 >\x0a\
+\x00\x00\x06\xe8\
+<\
+?xml version=\x221.\
+0\x22 encoding=\x22UTF\
+-8\x22 standalone=\x22\
+no\x22?>\x0a<svg\x0a   wi\
+dth=\x2248\x22\x0a   heig\
+ht=\x2248\x22\x0a   viewB\
+ox=\x220 0 48 48\x22\x0a \
+  version=\x221.1\x22\x0a\
+   id=\x22svg4\x22\x0a   \
+sodipodi:docname\
+=\x22cn_icon .svg\x22\x0a\
+   inkscape:vers\
+ion=\x221.1.2 (0a00\
+cf5339, 2022-02-\
+04)\x22\x0a   xmlns:in\
+kscape=\x22http://w\
+ww.inkscape.org/\
+namespaces/inksc\
+ape\x22\x0a   xmlns:so\
+dipodi=\x22http://s\
+odipodi.sourcefo\
+rge.net/DTD/sodi\
+podi-0.dtd\x22\x0a   x\
+mlns=\x22http://www\
+.w3.org/2000/svg\
+\x22\x0a   xmlns:svg=\x22\
+http://www.w3.or\
+g/2000/svg\x22\x0a   x\
+mlns:rdf=\x22http:/\
+/www.w3.org/1999\
+/02/22-rdf-synta\
+x-ns#\x22\x0a   xmlns:\
+cc=\x22http://creat\
+ivecommons.org/n\
+s#\x22\x0a   xmlns:dc=\
+\x22http://purl.org\
+/dc/elements/1.1\
+/\x22>\x0a  <metadata\x0a\
+     id=\x22metadat\
+a10\x22>\x0a    <rdf:R\
+DF>\x0a      <cc:Wo\
+rk\x0a         rdf:\
+about=\x22\x22>\x0a      \
+  <dc:format>ima\
+ge/svg+xml</dc:f\
+ormat>\x0a        <\
+dc:type\x0a        \
+   rdf:resource=\
+\x22http://purl.org\
+/dc/dcmitype/Sti\
+llImage\x22 />\x0a    \
+  </cc:Work>\x0a   \
+ </rdf:RDF>\x0a  </\
+metadata>\x0a  <def\
+s\x0a     id=\x22defs8\
+\x22 />\x0a  <sodipodi\
+:namedview\x0a     \
+pagecolor=\x22#ffff\
+ff\x22\x0a     borderc\
+olor=\x22#666666\x22\x0a \
+    borderopacit\
+y=\x221\x22\x0a     objec\
+ttolerance=\x2210\x22\x0a\
+     gridtoleran\
+ce=\x2210\x22\x0a     gui\
+detolerance=\x2210\x22\
+\x0a     inkscape:p\
+ageopacity=\x220\x22\x0a \
+    inkscape:pag\
+eshadow=\x222\x22\x0a    \
+ inkscape:window\
+-width=\x222505\x22\x0a  \
+   inkscape:wind\
+ow-height=\x221016\x22\
+\x0a     id=\x22namedv\
+iew6\x22\x0a     showg\
+rid=\x22false\x22\x0a    \
+ inkscape:zoom=\x22\
+4.2760417\x22\x0a     \
+inkscape:cx=\x22-0.\
+93544458\x22\x0a     i\
+nkscape:cy=\x2250.8\
+64799\x22\x0a     inks\
+cape:window-x=\x225\
+5\x22\x0a     inkscape\
+:window-y=\x2227\x22\x0a \
+    inkscape:win\
+dow-maximized=\x221\
+\x22\x0a     inkscape:\
+current-layer=\x22s\
+vg4\x22\x0a     inksca\
+pe:pagecheckerbo\
+ard=\x220\x22 />\x0a  <el\
+lipse\x0a     style\
+=\x22fill:#333333;f\
+ill-opacity:1;st\
+roke:#000000;str\
+oke-width:2.4;st\
+roke-linecap:rou\
+nd;stroke-linejo\
+in:round;stroke-\
+opacity:1;paint-\
+order:markers st\
+roke fill\x22\x0a     \
+id=\x22path848\x22\x0a   \
+  cx=\x2224.283655\x22\
+\x0a     cy=\x2225.593\
+718\x22\x0a     rx=\x226.\
+8985863\x22\x0a     ry\
+=\x227.1584754\x22 />\x0a\
+</svg>\x0a\
 \x00\x00\x14\xd4\
 \x00\
 \x01\xa6;x\xda\xed]\xddnc9r\xbe\xdf\xa7\x10\
 473X\x8bfU\xf1\xa7\xa8i\xcf\x02\xc1`\x93\
 \x5c,\x02dg\x12 7\x81F:\xb6\xb5#K\x86\
 \xa4n\xbb\xf7\xd5\xf2\x0ey\xa6\x14e[\x7f<\xce\xf4\
 2\xd8\x98f\xb3{\x1ac\x9f\x7f~\x1f\xc9\xafHV\
@@ -28021,14 +28326,18 @@
 \x083M\xc7\
 \x00s\
 \x00q\x00u\x00a\x00r\x00e\x00s\x00.\x00s\x00v\x00g\
 \x00\x0b\
 \x0d\x8e\x0eg\
 \x00a\
 \x00d\x00d\x00_\x00g\x00e\x00n\x00.\x00s\x00v\x00g\
+\x00\x10\
+\x05k\xa3g\
+\x00b\
+\x00u\x00s\x00_\x00b\x00a\x00r\x00_\x00i\x00c\x00o\x00n\x00.\x00s\x00v\x00g\
 \x00\x0f\
 \x08\xaa\x8f\xc7\
 \x00t\
 \x00i\x00m\x00e\x00_\x00s\x00e\x00r\x00i\x00e\x00s\x00.\x00s\x00v\x00g\
 \x00\x0d\
 \x0f\x18\xc9'\
 \x00c\
@@ -28201,14 +28510,18 @@
 \x05wT\xa7\
 \x00l\
 \x00o\x00a\x00d\x00.\x00s\x00v\x00g\
 \x00\x0b\
 \x0cT\xf1'\
 \x00t\
 \x00o\x00_\x00h\x00v\x00d\x00c\x00.\x00s\x00v\x00g\
+\x00\x0b\
+\x0a\xb5\xd1'\
+\x00c\
+\x00n\x00_\x00i\x00c\x00o\x00n\x00.\x00s\x00v\x00g\
 \x00\x16\
 \x06\x00\xa4\x07\
 \x00e\
 \x00x\x00p\x00a\x00n\x00s\x00i\x00o\x00n\x00_\x00p\x00l\x00a\x00n\x00n\x00i\x00n\
 \x00g\x00.\x00s\x00v\x00g\
 \x00\x0d\
 \x05\xe9:\xc7\
@@ -28395,311 +28708,315 @@
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x00\x00\x02\x00\x00\x00\x01\x00\x00\x00\x04\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00\x10\x00\x02\x00\x00\x00\x01\x00\x00\x00\x03\
 \x00\x00\x00\x00\x00\x00\x00\x00\
 \x00\x00\x00.\x00\x01\x00\x00\x00\x01\x00\x00\x00\x00\
 \x00\x00\x01\x8b\xd7}+v\
-\x00\x00\x00T\x00\x02\x00\x00\x00\x94\x00\x00\x00\x05\
+\x00\x00\x00T\x00\x02\x00\x00\x00\x96\x00\x00\x00\x05\
 \x00\x00\x00\x00\x00\x00\x00\x00\
-\x00\x00\x0c\xc2\x00\x00\x00\x00\x00\x01\x00\x04\xbb&\
+\x00\x00\x0c\xe8\x00\x00\x00\x00\x00\x01\x00\x04\xc7\x09\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0ab\x00\x00\x00\x00\x00\x01\x00\x03\xbd\x1d\
+\x00\x00\x0a\x88\x00\x00\x00\x00\x00\x01\x00\x03\xc9\x00\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x12:\x00\x00\x00\x00\x00\x01\x00\x06}\x09\
+\x00\x00\x12|\x00\x00\x00\x00\x00\x01\x00\x06\x8f\xd8\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x01\x00\x00\x00\x00\x00\x00\x01\x00\x00eu\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x094\x00\x00\x00\x00\x00\x01\x00\x03Z\xb7\
+\x00\x00\x09Z\x00\x00\x00\x00\x00\x01\x00\x03f\x9a\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x12^\x00\x00\x00\x00\x00\x01\x00\x06\x88\xae\
+\x00\x00\x12\xa0\x00\x00\x00\x00\x00\x01\x00\x06\x9b}\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x06\xe8\x00\x00\x00\x00\x00\x01\x00\x02\x8b\x88\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x05\x10\x00\x00\x00\x00\x00\x01\x00\x01\xf2\xd6\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x00\xd0\x00\x00\x00\x00\x00\x01\x00\x00N2\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x02\x18\x00\x00\x00\x00\x00\x01\x00\x00\xd0 \
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0e\x06\x00\x00\x00\x00\x00\x01\x00\x050z\
+\x00\x00\x0eH\x00\x00\x00\x00\x00\x01\x00\x05CI\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x11\xc8\x00\x00\x00\x00\x00\x01\x00\x06X<\
+\x00\x00\x12\x0a\x00\x00\x00\x00\x00\x01\x00\x06k\x0b\
 \x00\x00\x01\x8b\xd7}+z\
-\x00\x00\x0c:\x00\x00\x00\x00\x00\x01\x00\x04\x99$\
+\x00\x00\x0c`\x00\x00\x00\x00\x00\x01\x00\x04\xa5\x07\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0b\x84\x00\x00\x00\x00\x00\x01\x00\x043k\
+\x00\x00\x0b\xaa\x00\x00\x00\x00\x00\x01\x00\x04?N\
 \x00\x00\x01\x8d\x0d\x8c\x812\
 \x00\x00\x04\xba\x00\x00\x00\x00\x00\x01\x00\x01\xdc\x1e\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0e(\x00\x00\x00\x00\x00\x01\x00\x05:\x0f\
+\x00\x00\x0ej\x00\x00\x00\x00\x00\x01\x00\x05L\xde\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0e\x5c\x00\x01\x00\x00\x00\x01\x00\x05O\xa3\
+\x00\x00\x0e\x9e\x00\x01\x00\x00\x00\x01\x00\x05br\
 \x00\x00\x01\x8b\xd7}+z\
-\x00\x00\x10\xf2\x00\x00\x00\x00\x00\x01\x00\x06\x16\x0f\
+\x00\x00\x114\x00\x00\x00\x00\x00\x01\x00\x06(\xde\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x04\xa4\x00\x00\x00\x00\x00\x01\x00\x01\xccz\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x08\x80\x00\x01\x00\x00\x00\x01\x00\x03\x0d\x00\
+\x00\x00\x08\xa6\x00\x01\x00\x00\x00\x01\x00\x03\x18\xe3\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x04`\x00\x00\x00\x00\x00\x01\x00\x01\xac\xf1\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0a\x0c\x00\x00\x00\x00\x00\x01\x00\x03\x98U\
+\x00\x00\x0a2\x00\x00\x00\x00\x00\x01\x00\x03\xa48\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x00d\x00\x00\x00\x00\x00\x01\x00\x00\x11y\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x04\x82\x00\x00\x00\x00\x00\x01\x00\x01\xbd>\
 \x00\x00\x01\x8b\xd7}+z\
-\x00\x00\x0d\xd2\x00\x00\x00\x00\x00\x01\x00\x05\x0e\x8c\
+\x00\x00\x0e\x14\x00\x00\x00\x00\x00\x01\x00\x05![\
 \x00\x00\x01\x8e\x84\x8f\xee@\
 \x00\x00\x06\xb4\x00\x01\x00\x00\x00\x01\x00\x02{\xdb\
 \x00\x00\x01\x88\xae\xf9[%\
-\x00\x00\x12t\x00\x00\x00\x00\x00\x01\x00\x06\xa2\xcf\
+\x00\x00\x12\xb6\x00\x00\x00\x00\x00\x01\x00\x06\xb5\x9e\
 \x00\x00\x01\x8b\xd7}+z\
-\x00\x00\x0a\x82\x00\x01\x00\x00\x00\x01\x00\x03\xca\x0e\
+\x00\x00\x0a\xa8\x00\x01\x00\x00\x00\x01\x00\x03\xd5\xf1\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x00\xa4\x00\x00\x00\x00\x00\x01\x00\x004\x02\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x01(\x00\x00\x00\x00\x00\x01\x00\x00s\x90\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0f\xc2\x00\x00\x00\x00\x00\x01\x00\x05\xbcJ\
+\x00\x00\x10\x04\x00\x00\x00\x00\x00\x01\x00\x05\xcf\x19\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0f\x86\x00\x01\x00\x00\x00\x01\x00\x05\xa8|\
+\x00\x00\x0f\xc8\x00\x01\x00\x00\x00\x01\x00\x05\xbbK\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x09X\x00\x01\x00\x00\x00\x01\x00\x03c\xe7\
+\x00\x00\x09~\x00\x01\x00\x00\x00\x01\x00\x03o\xca\
 \x00\x00\x01\x8b\xd7}+z\
-\x00\x00\x08\xf0\x00\x00\x00\x00\x00\x01\x00\x03?\xd3\
+\x00\x00\x09\x16\x00\x00\x00\x00\x00\x01\x00\x03K\xb6\
 \x00\x00\x01\x8b\xd7}+~\
-\x00\x00\x0cz\x00\x01\x00\x00\x00\x01\x00\x04\xae\xf1\
+\x00\x00\x0c\xa0\x00\x01\x00\x00\x00\x01\x00\x04\xba\xd4\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x03\xaa\x00\x01\x00\x00\x00\x01\x00\x01gZ\
 \x00\x00\x01\x8b\xd7}+~\
-\x00\x00\x08\x94\x00\x00\x00\x00\x00\x01\x00\x03!\x88\
+\x00\x00\x08\xba\x00\x00\x00\x00\x00\x01\x00\x03-k\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0c\xe8\x00\x00\x00\x00\x00\x01\x00\x04\xc2\xbf\
+\x00\x00\x07\xd8\x00\x00\x00\x00\x00\x01\x00\x02\xd7\x19\
+\x00\x00\x01\x8e\xa3\x08\xbd\xac\
+\x00\x00\x0d\x0e\x00\x00\x00\x00\x00\x01\x00\x04\xce\xa2\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x09\x0c\x00\x01\x00\x00\x00\x01\x00\x03M%\
+\x00\x00\x092\x00\x01\x00\x00\x00\x01\x00\x03Y\x08\
 \x00\x00\x01\x88\xae\xf9[%\
 \x00\x00\x02\x80\x00\x01\x00\x00\x00\x01\x00\x00\xf2\xcc\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x070\x00\x00\x00\x00\x00\x01\x00\x02\xac\x07\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x082\x00\x00\x00\x00\x00\x01\x00\x02\xf2g\
+\x00\x00\x08X\x00\x00\x00\x00\x00\x01\x00\x02\xfeJ\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x06$\x00\x01\x00\x00\x00\x01\x00\x02R\xeb\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0dL\x00\x01\x00\x00\x00\x01\x00\x04\xea1\
+\x00\x00\x0d\x8e\x00\x01\x00\x00\x00\x01\x00\x04\xfd\x00\
 \x00\x00\x01\x88\xae\xf9[%\
-\x00\x00\x0d\x1a\x00\x01\x00\x00\x00\x01\x00\x04\xd5Y\
+\x00\x00\x0d\x5c\x00\x01\x00\x00\x00\x01\x00\x04\xe8(\
 \x00\x00\x01\x8b\xd7}+z\
 \x00\x00\x02d\x00\x00\x00\x00\x00\x01\x00\x00\xe2n\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x10\xd6\x00\x01\x00\x00\x00\x01\x00\x06\x08\x9c\
+\x00\x00\x11\x18\x00\x01\x00\x00\x00\x01\x00\x06\x1bk\
 \x00\x00\x01\x8b\xd7}+~\
 \x00\x00\x03|\x00\x01\x00\x00\x00\x01\x00\x01Tx\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x03P\x00\x01\x00\x00\x00\x01\x00\x01@\x19\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0a\xa4\x00\x00\x00\x00\x00\x01\x00\x03\xd1\xb0\
+\x00\x00\x0a\xca\x00\x00\x00\x00\x00\x01\x00\x03\xdd\x93\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x02\xe4\x00\x00\x00\x00\x00\x01\x00\x01 +\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x12\x1e\x00\x00\x00\x00\x00\x01\x00\x06os\
+\x00\x00\x12`\x00\x00\x00\x00\x00\x01\x00\x06\x82B\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x11j\x00\x00\x00\x00\x00\x01\x00\x06:\xa8\
+\x00\x00\x11\xac\x00\x00\x00\x00\x00\x01\x00\x06Mw\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x02\x98\x00\x00\x00\x00\x00\x01\x00\x00\xf7-\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x02:\x00\x01\x00\x00\x00\x01\x00\x00\xdbA\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0e\xa4\x00\x01\x00\x00\x00\x01\x00\x05\x5c4\
+\x00\x00\x0e\xe6\x00\x01\x00\x00\x00\x01\x00\x05o\x03\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x01<\x00\x00\x00\x00\x00\x01\x00\x00}9\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0b\xc8\x00\x00\x00\x00\x00\x01\x00\x04jc\
+\x00\x00\x0b\xee\x00\x00\x00\x00\x00\x01\x00\x04vF\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x00z\x00\x00\x00\x00\x00\x01\x00\x00\x1ac\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x11L\x00\x00\x00\x00\x00\x01\x00\x06/|\
+\x00\x00\x11\x8e\x00\x00\x00\x00\x00\x01\x00\x06BK\
 \x00\x00\x01\x8b\xd7}+~\
-\x00\x00\x08J\x00\x00\x00\x00\x00\x01\x00\x02\xf9\xf9\
+\x00\x00\x08p\x00\x00\x00\x00\x00\x01\x00\x03\x05\xdc\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x03\xfa\x00\x00\x00\x00\x00\x01\x00\x01{\xd6\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0e\xe4\x00\x00\x00\x00\x00\x01\x00\x05u\x93\
+\x00\x00\x0f&\x00\x00\x00\x00\x00\x01\x00\x05\x88b\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x01\x8e\x00\x01\x00\x00\x00\x01\x00\x00\xa2\xf8\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x06\x12\x00\x00\x00\x00\x00\x01\x00\x02C\xc6\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0f\xa4\x00\x00\x00\x00\x00\x01\x00\x05\xb1|\
+\x00\x00\x0f\xe6\x00\x00\x00\x00\x00\x01\x00\x05\xc4K\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x03\x98\x00\x01\x00\x00\x00\x01\x00\x01aP\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x10f\x00\x01\x00\x00\x00\x01\x00\x05\xe5u\
+\x00\x00\x10\xa8\x00\x01\x00\x00\x00\x01\x00\x05\xf8D\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x07\x02\x00\x00\x00\x00\x00\x01\x00\x02\x95\x8f\
 \x00\x00\x01\x8e.\xfc\xa1\x83\
-\x00\x00\x0eH\x00\x00\x00\x00\x00\x01\x00\x05E&\
+\x00\x00\x0e\x8a\x00\x00\x00\x00\x00\x01\x00\x05W\xf5\
 \x00\x00\x01\x88\xae\xf9[%\
 \x00\x00\x01\xc6\x00\x00\x00\x00\x00\x01\x00\x00\xae\xd1\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x09\xd2\x00\x00\x00\x00\x00\x01\x00\x03\x8c \
+\x00\x00\x09\xf8\x00\x00\x00\x00\x00\x01\x00\x03\x98\x03\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x052\x00\x00\x00\x00\x00\x01\x00\x02\x02{\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x02\xaa\x00\x00\x00\x00\x00\x01\x00\x00\xff\x1d\
 \x00\x00\x01\x88\xae\xf9[%\
 \x00\x00\x06x\x00\x00\x00\x00\x00\x01\x00\x02b\x90\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0dl\x00\x00\x00\x00\x00\x01\x00\x04\xf1N\
+\x00\x00\x0d\xae\x00\x00\x00\x00\x00\x01\x00\x05\x04\x1d\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x11(\x00\x00\x00\x00\x00\x01\x00\x06(\xb6\
+\x00\x00\x11j\x00\x00\x00\x00\x00\x01\x00\x06;\x85\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0b\xf2\x00\x00\x00\x00\x00\x01\x00\x04\x88(\
+\x00\x00\x0c\x18\x00\x00\x00\x00\x00\x01\x00\x04\x94\x0b\
 \x00\x00\x01\x8eL\x1c\xec)\
 \x00\x00\x07\xa0\x00\x00\x00\x00\x00\x01\x00\x02\xc2\xc9\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x05\xa8\x00\x00\x00\x00\x00\x01\x00\x02,!\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x10\xa2\x00\x01\x00\x00\x00\x01\x00\x05\xfb3\
+\x00\x00\x10\xe4\x00\x01\x00\x00\x00\x01\x00\x06\x0e\x02\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x11\x12\x00\x00\x00\x00\x00\x01\x00\x06 U\
+\x00\x00\x11T\x00\x00\x00\x00\x00\x01\x00\x063$\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x08\x1c\x00\x00\x00\x00\x00\x01\x00\x02\xec&\
+\x00\x00\x08B\x00\x00\x00\x00\x00\x01\x00\x02\xf8\x09\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x02\xd0\x00\x00\x00\x00\x00\x01\x00\x01\x0a0\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x07\xd8\x00\x00\x00\x00\x00\x01\x00\x02\xd7\x19\
+\x00\x00\x07\xfe\x00\x00\x00\x00\x00\x01\x00\x02\xe2\xfc\
 \x00\x00\x01\x8e.\xfc\xa1\x87\
-\x00\x00\x0a0\x00\x00\x00\x00\x00\x01\x00\x03\xaa\xdf\
+\x00\x00\x0aV\x00\x00\x00\x00\x00\x01\x00\x03\xb6\xc2\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x09\x1e\x00\x00\x00\x00\x00\x01\x00\x03S\x17\
+\x00\x00\x09D\x00\x00\x00\x00\x00\x01\x00\x03^\xfa\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0f2\x00\x00\x00\x00\x00\x01\x00\x05\x8aY\
+\x00\x00\x0ft\x00\x00\x00\x00\x00\x01\x00\x05\x9d(\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0b\xa4\x00\x00\x00\x00\x00\x01\x00\x04A\xfe\
+\x00\x00\x0b\xca\x00\x00\x00\x00\x00\x01\x00\x04M\xe1\
 \x00\x00\x01\x8b\xd7}+~\
-\x00\x00\x09\xea\x00\x01\x00\x00\x00\x01\x00\x03\x93\x9f\
+\x00\x00\x0a\x10\x00\x01\x00\x00\x00\x01\x00\x03\x9f\x82\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x10\x86\x00\x00\x00\x00\x00\x01\x00\x05\xf0*\
+\x00\x00\x10\xc8\x00\x00\x00\x00\x00\x01\x00\x06\x02\xf9\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x07Z\x00\x00\x00\x00\x00\x01\x00\x02\xb4\xb5\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x032\x00\x00\x00\x00\x00\x01\x00\x015\x01\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x11\xaa\x00\x00\x00\x00\x00\x01\x00\x06OY\
+\x00\x00\x11\xec\x00\x00\x00\x00\x00\x01\x00\x06b(\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x04\x0e\x00\x01\x00\x00\x00\x01\x00\x01\x87\xe2\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0b\xde\x00\x00\x00\x00\x00\x01\x00\x04z\x85\
+\x00\x00\x0c\x04\x00\x00\x00\x00\x00\x01\x00\x04\x86h\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x08\xb0\x00\x01\x00\x00\x00\x01\x00\x03*\xfa\
+\x00\x00\x08\xd6\x00\x01\x00\x00\x00\x01\x00\x036\xdd\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x00\x90\x00\x00\x00\x00\x00\x01\x00\x00!\xe4\
 \x00\x00\x01\x8b\xd7}+z\
-\x00\x00\x10F\x00\x01\x00\x00\x00\x01\x00\x05\xde\xab\
+\x00\x00\x10\x88\x00\x01\x00\x00\x00\x01\x00\x05\xf1z\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x04\xf2\x00\x00\x00\x00\x00\x01\x00\x01\xe8\x10\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x09\xa8\x00\x00\x00\x00\x00\x01\x00\x03~\xad\
+\x00\x00\x09\xce\x00\x00\x00\x00\x00\x01\x00\x03\x8a\x90\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0fj\x00\x00\x00\x00\x00\x01\x00\x05\x9ag\
+\x00\x00\x0f\xac\x00\x00\x00\x00\x00\x01\x00\x05\xad6\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x10\xba\x00\x00\x00\x00\x00\x01\x00\x05\xff\x88\
+\x00\x00\x10\xfc\x00\x00\x00\x00\x00\x01\x00\x06\x12W\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x05p\x00\x00\x00\x00\x00\x01\x00\x02\x10\xa0\
 \x00\x00\x01\x8d\x0d\x8c\x812\
-\x00\x00\x08\xd8\x00\x00\x00\x00\x00\x01\x00\x037]\
+\x00\x00\x08\xfe\x00\x00\x00\x00\x00\x01\x00\x03C@\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x06P\x00\x01\x00\x00\x00\x01\x00\x02Y\x19\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0bV\x00\x01\x00\x00\x00\x01\x00\x04,\xe7\
+\x00\x00\x0b|\x00\x01\x00\x00\x00\x01\x00\x048\xca\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x07\x88\x00\x00\x00\x00\x00\x01\x00\x02\xbb\xf6\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x06\xd2\x00\x00\x00\x00\x00\x01\x00\x02\x80\xad\
 \x00\x00\x01\x8b\xd7}+~\
 \x00\x00\x042\x00\x00\x00\x00\x00\x01\x00\x01\x8dL\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0c\x0a\x00\x00\x00\x00\x00\x01\x00\x04\x8fO\
+\x00\x00\x0d@\x00\x00\x00\x00\x00\x01\x00\x04\xe1<\
+\x00\x00\x01\x8e\xa3\x09s\x10\
+\x00\x00\x0c0\x00\x00\x00\x00\x00\x01\x00\x04\x9b2\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x01x\x00\x00\x00\x00\x00\x01\x00\x00\x9a\xd5\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x01V\x00\x01\x00\x00\x00\x01\x00\x00\x95\xeb\
 \x00\x00\x01\x8b\xd7}+z\
-\x00\x00\x0f\x04\x00\x01\x00\x00\x00\x01\x00\x05\x83A\
+\x00\x00\x0fF\x00\x01\x00\x00\x00\x01\x00\x05\x96\x10\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0e\xbc\x00\x00\x00\x00\x00\x01\x00\x05b\xee\
+\x00\x00\x0e\xfe\x00\x00\x00\x00\x00\x01\x00\x05u\xbd\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x00\xba\x00\x00\x00\x00\x00\x01\x00\x00@\xd4\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x01\xe4\x00\x01\x00\x00\x00\x01\x00\x00\xba\x91\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x04H\x00\x00\x00\x00\x00\x01\x00\x01\xa5\xd2\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0d\xbc\x00\x00\x00\x00\x00\x01\x00\x05\x05\x15\
+\x00\x00\x0d\xfe\x00\x00\x00\x00\x00\x01\x00\x05\x17\xe4\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0fH\x00\x01\x00\x00\x00\x01\x00\x05\x91\x95\
+\x00\x00\x0f\x8a\x00\x01\x00\x00\x00\x01\x00\x05\xa4d\
 \x00\x00\x01\x8b\xd7}+z\
 \x00\x00\x02\xfa\x00\x01\x00\x00\x00\x01\x00\x01)\x17\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0e\x86\x00\x01\x00\x00\x00\x01\x00\x05Vy\
+\x00\x00\x0e\xc8\x00\x01\x00\x00\x00\x01\x00\x05iH\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x06\xa0\x00\x00\x00\x00\x00\x01\x00\x02l\x97\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0c\xfe\x00\x00\x00\x00\x00\x01\x00\x04\xcaB\
+\x00\x00\x0d$\x00\x00\x00\x00\x00\x01\x00\x04\xd6%\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x10\x00\x00\x00\x00\x00\x00\x01\x00\x05\xcd\xe1\
+\x00\x00\x10B\x00\x00\x00\x00\x00\x01\x00\x05\xe0\xb0\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0aH\x00\x00\x00\x00\x00\x01\x00\x03\xb4\x10\
+\x00\x00\x0an\x00\x00\x00\x00\x00\x01\x00\x03\xbf\xf3\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0c\xaa\x00\x00\x00\x00\x00\x01\x00\x04\xb3E\
+\x00\x00\x0c\xd0\x00\x00\x00\x00\x00\x01\x00\x04\xbf(\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x05D\x00\x01\x00\x00\x00\x01\x00\x02\x09\xb0\
 \x00\x00\x01\x8e.\xfc\xa1\x83\
-\x00\x00\x0f\xea\x00\x00\x00\x00\x00\x01\x00\x05\xc6\x96\
+\x00\x00\x10,\x00\x00\x00\x00\x00\x01\x00\x05\xd9e\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x03\xd6\x00\x00\x00\x00\x00\x01\x00\x01n\xd8\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x10\x16\x00\x01\x00\x00\x00\x01\x00\x05\xd6[\
+\x00\x00\x10X\x00\x01\x00\x00\x00\x01\x00\x05\xe9*\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0a\xe8\x00\x00\x00\x00\x00\x01\x00\x03\xef\x88\
+\x00\x00\x0b\x0e\x00\x00\x00\x00\x00\x01\x00\x03\xfbk\
 \x00\x00\x01\x8b\xd7}+~\
-\x00\x00\x09\x88\x00\x01\x00\x00\x00\x01\x00\x03h\xf9\
+\x00\x00\x09\xae\x00\x01\x00\x00\x00\x01\x00\x03t\xdc\
 \x00\x00\x01\x8b\xd7}+z\
 \x00\x00\x07\xbc\x00\x00\x00\x00\x00\x01\x00\x02\xcap\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x03h\x00\x00\x00\x00\x00\x01\x00\x01F\x15\
 \x00\x00\x01\x88\xae\xf9[-\
 \x00\x00\x03\x18\x00\x01\x00\x00\x00\x01\x00\x01/\xd7\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0b\x0a\x00\x00\x00\x00\x00\x01\x00\x04\x0b\x87\
+\x00\x00\x0b0\x00\x00\x00\x00\x00\x01\x00\x04\x17j\
 \x00\x00\x01\x88\xae\xf9[%\
-\x00\x00\x0cb\x00\x00\x00\x00\x00\x01\x00\x04\xa1\xb5\
+\x00\x00\x0c\x88\x00\x00\x00\x00\x00\x01\x00\x04\xad\x98\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x0a\xc4\x00\x00\x00\x00\x00\x01\x00\x03\xe2I\
+\x00\x00\x0a\xea\x00\x00\x00\x00\x00\x01\x00\x03\xee,\
 \x00\x00\x01\x8b\xd7}+~\
-\x00\x00\x0d\x8c\x00\x01\x00\x00\x00\x01\x00\x04\xf9U\
+\x00\x00\x0d\xce\x00\x01\x00\x00\x00\x01\x00\x05\x0c$\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x00\xea\x00\x00\x00\x00\x00\x01\x00\x00Ze\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x11\xf4\x00\x01\x00\x00\x00\x01\x00\x06f\x11\
+\x00\x00\x126\x00\x01\x00\x00\x00\x01\x00\x06x\xe0\
 \x00\x00\x01\x8e.\xfc\xa1\x83\
 \x00\x00\x05\x84\x00\x00\x00\x00\x00\x01\x00\x02\x22i\
 \x00\x00\x01\x88\xae\xf9[-\
-\x00\x00\x07\xfc\x00\x00\x00\x00\x00\x01\x00\x02\xe1\x06\
+\x00\x00\x08\x22\x00\x00\x00\x00\x00\x01\x00\x02\xec\xe9\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x0b*\x00\x00\x00\x00\x00\x01\x00\x04\x14\xcb\
+\x00\x00\x0bP\x00\x00\x00\x00\x00\x01\x00\x04 \xae\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x08f\x00\x00\x00\x00\x00\x01\x00\x03\x02\xdf\
+\x00\x00\x08\x8c\x00\x00\x00\x00\x00\x01\x00\x03\x0e\xc2\
 \x00\x00\x01\x88\xae\xf9[)\
 \x00\x00\x05\xe4\x00\x00\x00\x00\x00\x01\x00\x029\xf9\
 \x00\x00\x01\x88\xae\xf9[)\
-\x00\x00\x11\x84\x00\x00\x00\x00\x00\x01\x00\x06B\x1a\
+\x00\x00\x11\xc6\x00\x00\x00\x00\x00\x01\x00\x06T\xe9\
 \x00\x00\x01\x8e.\xfc\xa1\x83\
 "
 
 def qInitResources():
     QtCore.qRegisterResourceData(0x03, qt_resource_struct, qt_resource_name, qt_resource_data)
 
 def qCleanupResources():
```

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/object_select_window.py` & `GridCal-5.1.1/GridCal/Gui/Main/object_select_window.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/SubClasses/simulations.py` & `GridCal-5.1.1/GridCal/Gui/Main/SubClasses/simulations.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # Engine imports
 import GridCalEngine.Devices as dev
 import GridCalEngine.Simulations as sim
 import GridCalEngine.Simulations.PowerFlow.grid_analysis as grid_analysis
 import GridCal.Gui.GuiFunctions as gf
 import GridCal.Gui.Visualization.visualization as viz
-from GridCal.Gui.BusBranchEditorWidget import BusBranchEditorWidget
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 from GridCalEngine.Compilers.circuit_to_newton_pa import get_newton_mip_solvers_list
 from GridCalEngine.Simulations.driver_types import SimulationTypes
 from GridCal.Gui.messages import yes_no_question, error_msg, warning_msg, info_msg
 from GridCal.Gui.Main.SubClasses.Model.time_events import TimeEventsMain
 from GridCal.Gui.SigmaAnalysis.sigma_analysis_dialogue import SigmaAnalysisGUI
 from GridCalEngine.Utils.MIP.selected_interface import get_available_mip_solvers
 from GridCalEngine.IO.file_system import get_create_gridcal_folder
```

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/SubClasses/io.py` & `GridCal-5.1.1/GridCal/Gui/Main/SubClasses/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 import GridCal.Gui.GuiFunctions as gf
 import GridCal.Session.export_results_driver as exprtdrv
 import GridCal.Session.file_handler as filedrv
 from GridCalEngine.Devices.multi_circuit import MultiCircuit
 from GridCal.Gui.CoordinatesInput.coordinates_dialogue import CoordinatesInputGUI
 from GridCal.Gui.GeneralDialogues import LogsDialogue, CustomQuestionDialogue
-from GridCal.Gui.BusBranchEditorWidget import BusBranchEditorWidget
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 from GridCal.Gui.messages import yes_no_question, error_msg, warning_msg, info_msg
 from GridCal.Gui.GridGenerator.grid_generator_dialogue import GridGeneratorGUI
 from GridCal.Gui.RosetaExplorer.RosetaExplorer import RosetaExplorerGUI
 from GridCal.Gui.Main.SubClasses.Settings.configuration import ConfigurationMain
 
 from GridCalEngine.Compilers.circuit_to_newton_pa import NEWTON_PA_AVAILABLE
 from GridCalEngine.Compilers.circuit_to_pgm import PGM_AVAILABLE
```

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/SubClasses/base_gui.py` & `GridCal-5.1.1/GridCal/Gui/Main/SubClasses/base_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 from GridCal.Gui.ProfilesInput.profile_dialogue import ProfileInputGUI
 from GridCal.Session.session import SimulationSession, GcThread
 from GridCal.Gui.SigmaAnalysis.sigma_analysis_dialogue import SigmaAnalysisGUI
 from GridCal.Gui.SyncDialogue.sync_dialogue import SyncDialogueWindow
 from GridCal.Gui.TowerBuilder.LineBuilderDialogue import TowerBuilderGUI
 from GridCal.Gui.GeneralDialogues import clear_qt_layout
 from GridCal.Gui.ConsoleWidget import ConsoleWidget
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import IS_DARK
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import IS_DARK
 from GridCal.templates import (get_cables_catalogue, get_transformer_catalogue, get_wires_catalogue,
                                get_sequence_lines_catalogue)
 
 
 def terminate_thread(thread):
     """Terminates a python thread from another thread.
```

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py` & `GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Scripting/python_highlighter.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Scripting/scripting.py` & `GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Scripting/scripting.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Settings/configuration.py` & `GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Settings/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 import os
 import qdarktheme
 from typing import Dict, Union
 from PySide6 import QtWidgets
 
 from GridCalEngine.IO.file_system import get_create_gridcal_folder
 from GridCal.Gui.Main.SubClasses.Results.results import ResultsMain
-from GridCal.Gui.BusBranchEditorWidget import BusBranchEditorWidget
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import set_dark_mode, set_light_mode
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import set_dark_mode, set_light_mode
 
 
 def config_data_to_struct(data_, struct_):
     """
     Recursive function to set the GUI values from the config dictionary
     :param data_: config dictionary with values from the file
     :param struct_: result of self.get_config_structure()
```

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Model/objects.py` & `GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Model/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from GridCalEngine.enumerations import DeviceType
 from GridCalEngine.Devices.types import ALL_DEV_TYPES
 from GridCal.Gui.Analysis.object_plot_analysis import object_histogram_analysis
 from GridCal.Gui.messages import yes_no_question, error_msg, warning_msg, info_msg
 from GridCal.Gui.Main.SubClasses.Model.diagrams import DiagramsMain
 from GridCal.Gui.TowerBuilder.LineBuilderDialogue import TowerBuilderGUI
 from GridCal.Gui.GeneralDialogues import LogsDialogue
-from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 from GridCal.Gui.SystemScaler.system_scaler import SystemScaler
 
 
 class ObjectsTableMain(DiagramsMain):
     """
     Diagrams Main
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Model/time_events.py` & `GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Model/time_events.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Model/diagrams.py` & `GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Model/diagrams.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 
 import GridCalEngine.Devices as dev
 import GridCalEngine.Simulations as sim
 import GridCal.Gui.GuiFunctions as gf
 import GridCal.Gui.Visualization.palettes as palettes
 from GridCalEngine.IO.file_system import get_create_gridcal_folder
 from GridCal.Gui.GeneralDialogues import CheckListDialogue, StartEndSelectionDialogue, InputSearchDialogue
-from GridCal.Gui.BusViewer.bus_viewer_dialogue import BusViewerWidget
-from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import (BusBranchEditorWidget,
-                                                                        BusGraphicItem,
-                                                                        generate_bus_branch_diagram)
-from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
-from GridCal.Gui.MapWidget.grid_map_widget import GridMapWidget
+from GridCal.Gui.Diagrams.BusViewer.bus_viewer_dialogue import BusViewerWidget
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import (BusBranchEditorWidget,
+                                                        BusGraphicItem,
+                                                        generate_bus_branch_diagram)
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+from GridCal.Gui.Diagrams.MapWidget.grid_map_widget import GridMapWidget
 from GridCal.Gui.messages import yes_no_question, error_msg, info_msg
 from GridCal.Gui.Main.SubClasses.Model.compiled_arrays import CompiledArraysMain
 from GridCal.Gui.Main.object_select_window import ObjectSelectWindow
-from GridCal.Gui.MapWidget.TileProviders.blue_marble import BlueMarbleTiles
-from GridCal.Gui.MapWidget.TileProviders.cartodb import CartoDbTiles
+from GridCal.Gui.Diagrams.MapWidget.TileProviders.blue_marble import BlueMarbleTiles
+from GridCal.Gui.Diagrams.MapWidget.TileProviders.cartodb import CartoDbTiles
 from GridCalEngine.Devices.types import ALL_DEV_TYPES
 
 ALL_EDITORS = Union[BusBranchEditorWidget, GridMapWidget, BusViewerWidget, NodeBreakerEditorWidget]
 ALL_EDITORS_NONE = Union[None, BusBranchEditorWidget, GridMapWidget, BusViewerWidget, NodeBreakerEditorWidget]
 
 
 class DiagramsMain(CompiledArraysMain):
```

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py` & `GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Model/compiled_arrays.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Main/SubClasses/Results/results.py` & `GridCal-5.1.1/GridCal/Gui/Main/SubClasses/Results/results.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Visualization/visualization.py` & `GridCal-5.1.1/GridCal/Gui/Visualization/visualization.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/Visualization/palettes.py` & `GridCal-5.1.1/GridCal/Gui/Visualization/palettes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Connector.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,37 +16,39 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 
 from enum import Enum
 import numpy as np
 from math import sqrt
 from PySide6 import QtGui
 from PySide6.QtCore import Qt, QPointF
-from PySide6.QtWidgets import QGraphicsLineItem, QGraphicsScene, QGraphicsRectItem, QGraphicsPathItem
+from PySide6.QtWidgets import QGraphicsScene, QGraphicsRectItem, QGraphicsPathItem
 
 
 class PlugOrganization(Enum):
     HORIZONTAL = 1
     VERTICAL = 2
     CIRCULAR = 3
 
+
 class Plug(QGraphicsRectItem):
-    def __init__(self, parent: QGraphicsScene, container = None, connector = None):
+    def __init__(self, parent: QGraphicsScene, container=None, connector=None):
         self.size = 10
         super().__init__(-self.size / 2, -self.size / 2, self.size, self.size)
         self.Parent = parent
         self.Container = container
         self.Connectors = list()
         self.setBrush(Qt.gray)
         self.Update()
         self.Parent.addItem(self)
 
     def Update(self):
         position = self.Container.scenePos()
         self.setPos(position.x(), position.y())
 
+
 class Connector(QGraphicsPathItem):
     def __init__(self, parent: QGraphicsScene, first: Plug, second: Plug):
         super().__init__()
         self.Parent = parent
         self.First = first
         self.Second = second
         self.Parent.addItem(self)
@@ -55,28 +57,28 @@
     def update(self):
         # Get the positions of the first and second objects
         first_pos = self.getPos(self.First)
         second_pos = self.getPos(self.Second)
 
         mid_x = first_pos.x() + ((second_pos.x() - first_pos.x()) * 0.5)
 
-
         path = QtGui.QPainterPath(QPointF(first_pos.x(), first_pos.y()))
         path.lineTo(mid_x, first_pos.y())
         path.lineTo(mid_x, second_pos.y())
         path.lineTo(second_pos.x(), second_pos.y())
 
         self.setPath(path)
 
         # Set the line's starting and ending points
         # self.setLine(first_pos.x(), first_pos.y(), second_pos.x(), second_pos.y())
 
     def getPos(self, element):
         return element.scenePos()
 
+
 class ConnectionManager:
     def __init__(self):
         self.PlugList = list()
         self.FirstConnector = None
         self.SecondConnector = None
         self.minimumDistance = 50
 
@@ -105,44 +107,45 @@
 
     def SetSecondConnector(self, xPos: float, yPos: float):
         self.SecondConnector = self.FindNearestConnector(xPos, yPos)
 
     def CreateConnection(self, parent: QGraphicsScene):
         print(self.FirstConnector)
         print(self.SecondConnector)
-        if(self.FirstConnector != None and self.SecondConnector != None):
+        if (self.FirstConnector != None and self.SecondConnector != None):
             if (self.FirstConnector.Container != self.SecondConnector.Container
-                and self.FirstConnector != self.SecondConnector):
+                    and self.FirstConnector != self.SecondConnector):
                 newConnector = Connector(parent, self.FirstConnector, self.SecondConnector)
                 self.FirstConnector.Container.Connection.Connectors.append(newConnector)
                 self.SecondConnector.Container.Connection.Connectors.append(newConnector)
                 self.FirstConnector.Connectors.append(newConnector)
                 self.SecondConnector.Connectors.append(newConnector)
         self.FirstConnector = None
         self.SecondConnector = None
 
+
 class ConnectionItem:
-    def __init__(self, parent: QGraphicsScene, manager: ConnectionManager, container = None, organization = 3):
+    def __init__(self, parent: QGraphicsScene, manager: ConnectionManager, container=None, organization=3):
         self.Parent = parent
         self.Manager = manager
         self.Container = container
         self.Connectors = list()
         self.Organization = organization
         # Plugs
         self.PlugList = list()
         self.UpdatePlugs()
 
-    def CreatePlugs(self, number = 1, updateModel = True):
+    def CreatePlugs(self, number=1, updateModel=True):
         self.PlugList.clear()
         for i in range(number):
             newPlug = Plug(self.Parent, self.Container, None)
             """Add a Plug object to the Bus and arrange it vertically."""
             self.PlugList.append(newPlug)
             newPlug.setParentItem(self.Container)
-            if(updateModel):
+            if (updateModel):
                 self.UpdatePlugs()
             self.Manager.PlugList.append(newPlug)
 
     def UpdatePlugs(self):
         if len(self.PlugList) > 0:
             if self.Organization == 2:
                 bus_height = self.Container.rect().height()
@@ -173,10 +176,7 @@
                 for i, plug in enumerate(self.PlugList):
                     plug.setPos(xt[i], yt[i])
 
     def Update(self):
         self.UpdatePlugs()
         for connector in self.Connectors:
             connector.update()
-
-
-
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/node_breaker_editor_widget.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/node_breaker_editor_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from PySide6.QtGui import (QIcon, QPixmap, QImage, QPainter, QStandardItemModel, QStandardItem, QColor, QPen,
                            QDragEnterEvent, QDragMoveEvent, QDropEvent, QWheelEvent, QKeyEvent, QDrag)
 from PySide6.QtWidgets import (QApplication, QGraphicsView, QListView, QTableView, QVBoxLayout, QHBoxLayout, QFrame,
                                QSplitter, QMessageBox, QAbstractItemView, QGraphicsScene, QGraphicsSceneMouseEvent,
                                QGraphicsItem)
 from PySide6.QtSvg import QSvgGenerator
 
-from GridCal.Gui.NodeBreakerEditorWidget.Connector import Connector, Plug, ConnectionManager
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Connector import Connector, Plug, ConnectionManager
 from GridCalEngine.Devices.multi_circuit import MultiCircuit
 from GridCalEngine.Devices.Substation import Bus
 from GridCalEngine.Devices.Parents.editable_device import EditableDevice
 from GridCalEngine.Devices.Branches.line import Line
 from GridCalEngine.Devices.Branches.dc_line import DcLine
 from GridCalEngine.Devices.Branches.transformer import Transformer2W
 from GridCalEngine.Devices.Branches.vsc import VSC
@@ -48,28 +48,28 @@
 from GridCalEngine.Simulations.driver_types import SimulationTypes
 from GridCalEngine.Simulations.driver_template import DriverTemplate
 from GridCalEngine.Devices.Diagrams.node_breaker_diagram import NodeBreakerDiagram
 from GridCalEngine.Devices.Diagrams.graphic_location import GraphicLocation
 from GridCalEngine.basic_structures import Vec, CxVec, IntVec
 from GridCalEngine.Devices.types import ALL_DEV_TYPES
 
-from GridCal.Gui.NodeBreakerEditorWidget.terminal_item import TerminalItem
-from GridCal.Gui.NodeBreakerEditorWidget.Substation.bus_graphics import BusGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Fluid.fluid_node_graphics import FluidNodeGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Fluid.fluid_path_graphics import FluidPathGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.line_graphics import LineGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.winding_graphics import WindingGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.dc_line_graphics import DcLineGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.transformer2w_graphics import TransformerGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.hvdc_graphics import HvdcGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.vsc_graphics import VscGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.upfc_graphics import UpfcGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.Rectangle_Connector import RectangleConnectorGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.generator_graphics import GeneratorGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.terminal_item import TerminalItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Substation.bus_graphics import BusGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Fluid.fluid_node_graphics import FluidNodeGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Fluid.fluid_path_graphics import FluidPathGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.line_graphics import LineGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.winding_graphics import WindingGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.dc_line_graphics import DcLineGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.transformer2w_graphics import TransformerGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.hvdc_graphics import HvdcGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.vsc_graphics import VscGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.upfc_graphics import UpfcGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.Rectangle_Connector import RectangleConnectorGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.generator_graphics import GeneratorGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE
 import GridCal.Gui.Visualization.visualization as viz
 import GridCal.Gui.Visualization.palettes as palettes
 from GridCal.Gui.messages import info_msg
 from GridCal.Gui.GuiFunctions import ObjectsModel
 from matplotlib import pyplot as plt
 
 '''
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/generic_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/generic_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/matplotlibwidget.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/matplotlibwidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/terminal_item.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/terminal_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from typing import Union
 from PySide6.QtCore import Qt, QPointF, QRectF, QRect
 from PySide6.QtGui import QPen, QCursor
 from PySide6.QtWidgets import QGraphicsRectItem, QGraphicsItem, QGraphicsEllipseItem
 
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE
 
 
 class TerminalItem(QGraphicsRectItem):
     """
     Represents a connection point to a subsystem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Fluid/fluid_turbine_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Fluid/fluid_turbine_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtCore import QPointF
 from PySide6.QtGui import QPen, QIcon, QPixmap
 from PySide6.QtWidgets import (QMenu, QGraphicsTextItem, QGraphicsSceneMouseEvent)
 from GridCalEngine.enumerations import DeviceType
 from GridCalEngine.Devices.Fluid.fluid_turbine import FluidTurbine
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
 from GridCal.Gui.GuiFunctions import ObjectsModel
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class FluidTurbineGraphicItem(InjectionTemplateGraphicItem):
     """
     FluidTurbineGraphicItem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Fluid/fluid_pump_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Fluid/fluid_pump_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtCore import QPointF
 from PySide6.QtGui import QPen, QIcon, QPixmap
 from PySide6.QtWidgets import (QMenu, QGraphicsTextItem)
 from GridCalEngine.Devices.Fluid.fluid_pump import FluidPump
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class FluidPumpGraphicItem(InjectionTemplateGraphicItem):
     """
     FluidPumpGraphicItem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Fluid/fluid_path_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Fluid/fluid_path_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import Union, TYPE_CHECKING
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QPen, QIcon, QPixmap, QColor
 from PySide6.QtWidgets import QMenu
 from GridCal.Gui.GeneralDialogues import InputNumberDialogue
-from GridCal.Gui.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.line_editor import LineEditor
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.line_editor import LineEditor
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE
 from GridCalEngine.Devices.Fluid.fluid_path import FluidPath
 from GridCalEngine.enumerations import DeviceType
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class FluidPathGraphicItem(LineGraphicTemplateItem):
     """
     LineGraphicItem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Fluid/fluid_p2x_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Fluid/fluid_p2x_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtCore import QPointF
 from PySide6.QtGui import QPen, QIcon, QPixmap
 from PySide6.QtWidgets import (QMenu, QGraphicsTextItem)
 from GridCalEngine.Devices.Fluid.fluid_p2x import FluidP2x
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class FluidP2xGraphicItem(InjectionTemplateGraphicItem):
     """
     FluidP2xGraphicItem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Fluid/fluid_node_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Fluid/fluid_node_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 import numpy as np
 from typing import Union, TYPE_CHECKING
 from PySide6 import QtWidgets
 from PySide6.QtCore import Qt, QPoint
 from PySide6.QtGui import QPen, QCursor, QIcon, QPixmap, QBrush
 from PySide6.QtWidgets import QMenu, QGraphicsScene, QGraphicsSceneMouseEvent
 
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, FONT_SCALE
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, FONT_SCALE
 from GridCal.Gui.GuiFunctions import ObjectsModel
 from GridCalEngine.Devices.Fluid import FluidNode, FluidTurbine, FluidPump, FluidP2x
 from GridCalEngine.Devices.Substation.bus import Bus
-from GridCal.Gui.NodeBreakerEditorWidget.terminal_item import TerminalItem, HandleItem
-from GridCal.Gui.NodeBreakerEditorWidget.Fluid.fluid_turbine_graphics import FluidTurbineGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Fluid.fluid_pump_graphics import FluidPumpGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Fluid.fluid_p2x_graphics import FluidP2xGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.terminal_item import TerminalItem, HandleItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Fluid.fluid_turbine_graphics import FluidTurbineGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Fluid.fluid_pump_graphics import FluidPumpGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Fluid.fluid_p2x_graphics import FluidP2xGraphicItem
 from GridCal.Gui.messages import yes_no_question
 from GridCalEngine.enumerations import DeviceType, FaultType
 from GridCalEngine.Devices.Parents.editable_device import EditableDevice
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class FluidNodeGraphicItem(QtWidgets.QGraphicsRectItem):
     """
       Represents a block in the diagram
       Has an x and y and width and height
       width and height can only be adjusted with a tip in the lower right corner.
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/winding_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/winding_graphics.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
 from GridCal.Gui.messages import yes_no_question
 from GridCalEngine.Devices.Branches.winding import Winding
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class WindingGraphicItem(LineGraphicTemplateItem):
 
     def __init__(self,
                  fromPort: TerminalItem,
                  toPort: Union[TerminalItem, None],
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/line_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/line_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,23 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union
 from PySide6.QtCore import Qt, QRectF
 from PySide6.QtGui import QPen, QIcon, QPixmap, QBrush
 from PySide6.QtWidgets import QMenu, QGraphicsRectItem
 from GridCal.Gui.GeneralDialogues import InputNumberDialogue
-from GridCal.Gui.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.line_editor import LineEditor
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.line_editor import LineEditor
 from GridCal.Gui.messages import yes_no_question, warning_msg
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 from GridCalEngine.Devices.Branches.line import Line, SequenceLineType
 from GridCalEngine.enumerations import DeviceType
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class LineGraphicItem(LineGraphicTemplateItem):
     """
     LineGraphicItem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/switch_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/switch_graphics.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/dc_line_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/dc_line_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 import numpy as np
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu, QLabel, QDoubleSpinBox, QPushButton, QVBoxLayout, QComboBox, QDialog, QGraphicsScene
 from GridCal.Gui.GuiFunctions import get_list_model
-from GridCal.Gui.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
 from GridCalEngine.Devices.Branches.line import SequenceLineType, OverheadLineType, UndergroundLineType
 from GridCalEngine.Devices.Branches.dc_line import DcLine
 from GridCalEngine.enumerations import DeviceType
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class DcLineEditor(QDialog):
     """
     DcLineEditor
     """
     def __init__(self, branch: DcLine, Sbase=100, templates=None, current_template=None):
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/hvdc_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/hvdc_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
 from GridCalEngine.Devices.Branches.hvdc_line import HvdcLine
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class HvdcGraphicItem(LineGraphicTemplateItem):
 
     def __init__(self, fromPort: TerminalItem, toPort: TerminalItem,
                  editor: NodeBreakerEditorWidget, width=5,
                  api_object: HvdcLine = None):
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/upfc_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/vsc_graphics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 # GridCal
 # Copyright (C) 2015 - 2024 Santiago Peñate Vera
-# 
+#
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 3 of the License, or (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
-from GridCalEngine.Devices.Branches.upfc import UPFC
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCalEngine.Devices.Branches.vsc import VSC
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
-class UpfcGraphicItem(LineGraphicTemplateItem):
+class VscGraphicItem(LineGraphicTemplateItem):
+    """
+    Graphics item for the VSC converter
+    """
 
     def __init__(self, fromPort: TerminalItem, toPort: TerminalItem,
                  editor: NodeBreakerEditorWidget, width=5,
-                 api_object: UPFC = None):
+                 api_object: VSC = None):
         """
 
         :param fromPort:
         :param toPort:
         :param editor:
         :param width:
         :param api_object:
@@ -105,7 +108,16 @@
             re_icon.addPixmap(QPixmap(":/Icons/icons/grid_reduction.svg"))
             re.setIcon(re_icon)
             re.triggered.connect(self.reduce)
 
             menu.exec_(event.screenPos())
         else:
             pass
+
+    def mouseDoubleClickEvent(self, event):
+        """
+        On double click, edit
+        :param event:
+        :return:
+        """
+
+        pass
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/transformer2w_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/transformer2w_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu, QGraphicsScene
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
-from GridCal.Gui.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.transformer_editor import TransformerEditor, reverse_transformer_short_circuit_study
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.transformer_editor import TransformerEditor, reverse_transformer_short_circuit_study
 from GridCalEngine.Devices.Branches.transformer import Transformer2W, TransformerType
 from GridCalEngine.enumerations import DeviceType
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class TransformerGraphicItem(LineGraphicTemplateItem):
     """
     TransformerGraphicItem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/line_editor.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/line_editor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/vsc_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/upfc_graphics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 # GridCal
 # Copyright (C) 2015 - 2024 Santiago Peñate Vera
-#
+# 
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 3 of the License, or (at your option) any later version.
-#
+# 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
-#
+# 
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
-from GridCalEngine.Devices.Branches.vsc import VSC
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCalEngine.Devices.Branches.upfc import UPFC
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
-class VscGraphicItem(LineGraphicTemplateItem):
-    """
-    Graphics item for the VSC converter
-    """
+class UpfcGraphicItem(LineGraphicTemplateItem):
 
     def __init__(self, fromPort: TerminalItem, toPort: TerminalItem,
                  editor: NodeBreakerEditorWidget, width=5,
-                 api_object: VSC = None):
+                 api_object: UPFC = None):
         """
 
         :param fromPort:
         :param toPort:
         :param editor:
         :param width:
         :param api_object:
@@ -108,16 +105,7 @@
             re_icon.addPixmap(QPixmap(":/Icons/icons/grid_reduction.svg"))
             re.setIcon(re_icon)
             re.triggered.connect(self.reduce)
 
             menu.exec_(event.screenPos())
         else:
             pass
-
-    def mouseDoubleClickEvent(self, event):
-        """
-        On double click, edit
-        :param event:
-        :return:
-        """
-
-        pass
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/transformer_editor.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/transformer_editor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/Rectangle_Connector.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/Rectangle_Connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,24 +18,24 @@
 import numpy as np
 from typing import List, TYPE_CHECKING
 from PySide6.QtCore import Qt, QPoint, QPointF
 from PySide6.QtGui import QPen, QCursor, QColor, QIcon, QPixmap
 from PySide6.QtWidgets import QGraphicsItem, QGraphicsEllipseItem, QGraphicsRectItem, QMenu, QGraphicsSceneMouseEvent, \
     QGraphicsTextItem
 
-from GridCal.Gui.NodeBreakerEditorWidget.Connector import ConnectionItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Connector import ConnectionItem
 from GridCalEngine.Devices.Branches.transformer3w import Transformer3W
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED
 from GridCal.Gui.GuiFunctions import ObjectsModel
-from GridCal.Gui.NodeBreakerEditorWidget.terminal_item import TerminalItem
-from GridCal.Gui.NodeBreakerEditorWidget.Branches.winding_graphics import WindingGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.terminal_item import TerminalItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Branches.winding_graphics import WindingGraphicItem
 from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class RectangleConnectorGraphicItem(QGraphicsRectItem):
     """
       Represents a block in the diagram
       Has an x and y and width and height
       width and height can only be adjusted with a tip in the lower right corner.
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Branches/line_graphics_template.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Branches/line_graphics_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 import sys
 import numpy as np
 from typing import Union, TYPE_CHECKING
 from PySide6.QtCore import Qt, QLineF, QPointF, QRectF
 from PySide6.QtGui import QPen, QCursor, QPixmap, QBrush, QColor, QTransform, QPolygonF
 from PySide6.QtWidgets import (QGraphicsLineItem, QGraphicsRectItem, QGraphicsPolygonItem,
                                QGraphicsEllipseItem, QGraphicsSceneMouseEvent)
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER
-from GridCal.Gui.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
-from GridCal.Gui.NodeBreakerEditorWidget.Substation.bus_graphics import BusGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Fluid.fluid_node_graphics import FluidNodeGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Substation.bus_graphics import BusGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Fluid.fluid_node_graphics import FluidNodeGraphicItem
 
 from GridCal.Gui.messages import yes_no_question, warning_msg, error_msg
 from GridCal.Gui.GuiFunctions import ObjectsModel
 from GridCalEngine.Devices.Substation.bus import Bus
 from GridCalEngine.Devices.Branches.line import Line
 from GridCalEngine.Devices.Branches.transformer import Transformer2W
 from GridCalEngine.Devices.Branches.vsc import VSC
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/static_generator_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/static_generator_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import Union, TYPE_CHECKING
 from PySide6.QtGui import QPen, QIcon, QPixmap
 from PySide6.QtWidgets import QMenu, QGraphicsTextItem
 from GridCalEngine.Devices.Injections.static_generator import StaticGenerator, DeviceType
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.GuiFunctions import ObjectsModel
 from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class StaticGeneratorGraphicItem(InjectionTemplateGraphicItem):
 
     def __init__(self, parent, api_obj: StaticGenerator, editor: "NodeBreakerEditorWidget"):
         """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/injections_template_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/injections_template_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QPen, QCursor
 from PySide6.QtWidgets import QGraphicsLineItem, QGraphicsItemGroup
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER
 from GridCal.Gui.messages import yes_no_question, error_msg, warning_msg
 from GridCalEngine.enumerations import DeviceType
 from GridCalEngine.Devices.types import INJECTION_DEVICE_TYPES
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class InjectionTemplateGraphicItem(QGraphicsItemGroup):
     """
     InjectionTemplateGraphicItem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/battery_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/battery_graphics.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6 import QtWidgets, QtGui
 from GridCalEngine.Devices.Injections.battery import Battery, DeviceType
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.GuiFunctions import ObjectsModel
 from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class BatteryGraphicItem(InjectionTemplateGraphicItem):
 
     def __init__(self, parent, api_obj: Battery, editor: NodeBreakerEditorWidget):
         """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/shunt_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/shunt_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6 import QtWidgets
 from PySide6.QtCore import QPointF, QLineF
 from PySide6.QtGui import QPen, QIcon, QPixmap
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Line
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Line
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class ShuntGraphicItem(InjectionTemplateGraphicItem):
 
     def __init__(self, parent, api_obj, editor: "NodeBreakerEditorWidget"):
         """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/external_grid_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/external_grid_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6 import QtWidgets, QtGui, QtCore
 from GridCalEngine.Devices.Injections.battery import Battery, DeviceType
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.GuiFunctions import ObjectsModel
 from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class ExternalGridGraphicItem(InjectionTemplateGraphicItem):
     """
     ExternalGrid graphic item
     """
     def __init__(self, parent, api_obj: Battery, editor: NodeBreakerEditorWidget):
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/load_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/load_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtCore import QPointF
 from PySide6.QtGui import QPen, QIcon, QPixmap, QPolygonF
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import Polygon
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import Polygon
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class LoadGraphicItem(InjectionTemplateGraphicItem):
 
     def __init__(self, parent, api_obj, editor: NodeBreakerEditorWidget):
         """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Injections/generator_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Injections/generator_graphics.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 from PySide6.QtCore import Qt, QAbstractTableModel, QModelIndex, QPointF
 from PySide6.QtGui import QPen, QIcon, QPixmap
 from PySide6.QtWidgets import (QMenu, QGraphicsTextItem, QDialog, QTableView, QVBoxLayout, QHBoxLayout,
                                QPushButton, QSplitter, QFrame, QSpacerItem, QSizePolicy)
 from GridCalEngine.Devices.Injections.generator import Generator
 from GridCalEngine.Devices.Injections.generator_q_curve import GeneratorQCurve
 from GridCalEngine.basic_structures import Mat, Vec
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
-from GridCal.Gui.NodeBreakerEditorWidget.matplotlibwidget import MatplotlibWidget
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.matplotlibwidget import MatplotlibWidget
 from GridCal.Gui.messages import yes_no_question, info_msg
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.SolarPowerWizard.solar_power_wizzard import SolarPvWizard
 from GridCal.Gui.WindPowerWizard.wind_power_wizzard import WindFarmWizard
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
+    from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
 
 
 class GeneratorQCurveEditorTableModel(QAbstractTableModel):
     """
     GeneratorQCurveEditorTableModel
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/NodeBreakerEditorWidget/Substation/bus_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/NodeBreakerEditorWidget/Substation/bus_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,26 +18,26 @@
 import numpy as np
 from typing import Union, TYPE_CHECKING
 from PySide6 import QtWidgets
 from PySide6.QtCore import Qt, QPoint, QRectF, QRect
 from PySide6.QtGui import QPen, QCursor, QIcon, QPixmap, QBrush, QColor
 from PySide6.QtWidgets import QMenu, QGraphicsSceneMouseEvent
 
-from GridCal.Gui.NodeBreakerEditorWidget.Connector import ConnectionItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Connector import ConnectionItem
 from GridCalEngine.Devices.Substation import Bus
-from GridCal.Gui.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, FONT_SCALE, EMERGENCY
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, FONT_SCALE, EMERGENCY
 from GridCal.Gui.GuiFunctions import ObjectsModel
 from GridCalEngine.Simulations.Topology.topology_reduction_driver import reduce_buses
-from GridCal.Gui.NodeBreakerEditorWidget.terminal_item import TerminalItem, HandleItem
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.load_graphics import LoadGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.generator_graphics import GeneratorGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.static_generator_graphics import StaticGeneratorGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.battery_graphics import BatteryGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.shunt_graphics import ShuntGraphicItem
-from GridCal.Gui.NodeBreakerEditorWidget.Injections.external_grid_graphics import ExternalGridGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.terminal_item import TerminalItem, HandleItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.load_graphics import LoadGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.generator_graphics import GeneratorGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.static_generator_graphics import StaticGeneratorGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.battery_graphics import BatteryGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.shunt_graphics import ShuntGraphicItem
+from GridCal.Gui.Diagrams.NodeBreakerEditorWidget.Injections.external_grid_graphics import ExternalGridGraphicItem
 from GridCal.Gui.messages import yes_no_question
 from GridCalEngine.enumerations import DeviceType, FaultType
 from GridCalEngine.Devices.Parents.editable_device import EditableDevice
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
     from GridCal.Gui.NodeBreakerEditorWidget.node_breaker_editor_widget import NodeBreakerEditorWidget
```

### Comparing `GridCal-5.1.0/GridCal/Gui/SyncDialogue/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/SyncDialogue/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/SyncDialogue/sync_dialogue.py` & `GridCal-5.1.1/GridCal/Gui/SyncDialogue/sync_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/SyncDialogue/gui.py` & `GridCal-5.1.1/GridCal/Gui/SyncDialogue/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py` & `GridCal-5.1.1/GridCal/Gui/SolarPowerWizard/solar_power_wizzard.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/SolarPowerWizard/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/SolarPowerWizard/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/SolarPowerWizard/gui.py` & `GridCal-5.1.1/GridCal/Gui/SolarPowerWizard/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/map_widget.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/map_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 import math
 from typing import List, Dict, Union, Tuple, Callable
 from PySide6.QtCore import Qt, QTimer, QPoint, QPointF, QEvent
 from PySide6.QtWidgets import QSizePolicy, QWidget, QMessageBox, QGraphicsScene, QGraphicsView, QVBoxLayout
 from PySide6.QtGui import QPainter, QColor, QPixmap, QPen, QFont, QFontMetrics, QPolygon, QBrush, QCursor, \
     QMouseEvent, QKeyEvent, QWheelEvent, QResizeEvent, QEnterEvent, QPaintEvent
 
-from GridCal.Gui.MapWidget.Schema.SchemaManager import schemaManager
-from GridCal.Gui.MapWidget.map_events import LevelEvent, PositionEvent, SelectEvent, BoxSelectEvent
-from GridCal.Gui.MapWidget.logger import log
-from GridCal.Gui.MapWidget.Layers.point_layer import PointLayer, PointData
-from GridCal.Gui.MapWidget.Layers.polygon_layer import PolygonLayer, PolygonData
-from GridCal.Gui.MapWidget.Layers.polyline_layer import PolylineLayer, PolylineData
-from GridCal.Gui.MapWidget.Layers.text_layer import TextLayer, TextData
-from GridCal.Gui.MapWidget.Layers.image_layer import ImageLayer, ImageData
-from GridCal.Gui.MapWidget.Layers.layer_types import LayerType
-from GridCal.Gui.MapWidget.Layers.place import Place
-from GridCal.Gui.MapWidget.Tiles.tiles import Tiles
+from GridCal.Gui.Diagrams.MapWidget.Schema.SchemaManager import schemaManager
+from GridCal.Gui.Diagrams.MapWidget.map_events import LevelEvent, PositionEvent, SelectEvent, BoxSelectEvent
+from GridCal.Gui.Diagrams.MapWidget.logger import log
+from GridCal.Gui.Diagrams.MapWidget.Layers.point_layer import PointLayer, PointData
+from GridCal.Gui.Diagrams.MapWidget.Layers.polygon_layer import PolygonLayer, PolygonData
+from GridCal.Gui.Diagrams.MapWidget.Layers.polyline_layer import PolylineLayer, PolylineData
+from GridCal.Gui.Diagrams.MapWidget.Layers.text_layer import TextLayer, TextData
+from GridCal.Gui.Diagrams.MapWidget.Layers.image_layer import ImageLayer, ImageData
+from GridCal.Gui.Diagrams.MapWidget.Layers.layer_types import LayerType
+from GridCal.Gui.Diagrams.MapWidget.Layers.place import Place
+from GridCal.Gui.Diagrams.MapWidget.Tiles.tiles import Tiles
 
 # version number of the widget
 __version__ = '0.5'
 
 from GridCalEngine.IO.matpower.matpower_branch_definitions import QT
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/node_widget.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/node_widget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/map_events.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/map_events.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/grid_map_widget.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/grid_map_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,30 +14,32 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from typing import Union, List
 import numpy as np
 from PySide6.QtWidgets import QWidget
 from collections.abc import Callable
-from GridCal.Gui.MapWidget.map_widget import MapWidget, PolylineData, Place
-import GridCal.Gui.Visualization.visualization as viz
-import GridCal.Gui.Visualization.palettes as palettes
+
 from GridCalEngine.Devices.Diagrams.map_location import MapLocation
 from GridCalEngine.Devices.Substation import Bus
 from GridCalEngine.Devices.Branches.line import Line
 from GridCalEngine.Devices.Branches.dc_line import DcLine
 from GridCalEngine.Devices.Branches.hvdc_line import HvdcLine
 from GridCalEngine.Devices.Diagrams.map_diagram import MapDiagram
 from GridCalEngine.Devices.types import BRANCH_TYPES
 from GridCalEngine.Devices.Fluid import FluidNode, FluidPath
 from GridCalEngine.basic_structures import Vec, CxVec, IntVec
 from GridCalEngine.Devices.Substation.substation import Substation
 from GridCalEngine.Devices.Substation.voltage_level import VoltageLevel
 
-from GridCal.Gui.MapWidget.Tiles.tiles import Tiles
+from GridCal.Gui.Diagrams.MapWidget.map_widget import MapWidget, PolylineData, Place
+import GridCal.Gui.Visualization.visualization as viz
+import GridCal.Gui.Visualization.palettes as palettes
+from GridCal.Gui.Diagrams.graphics_manager import GraphicsManager
+from GridCal.Gui.Diagrams.MapWidget.Tiles.tiles import Tiles
 
 
 class GridMapWidget(MapWidget):
 
     def __init__(self,
                  parent: Union[QWidget, None],
                  tile_src: Tiles,
@@ -50,14 +52,16 @@
         MapWidget.__init__(self,
                            parent=parent,
                            tile_src=tile_src,
                            start_level=start_level,
                            zoom_callback=self.zoom_callback,
                            position_callback=self.position_callback)
 
+        self.graphics_manager = GraphicsManager()
+
         # diagram to store the objects locations
         self.diagram: MapDiagram = MapDiagram(name=name,
                                               tile_source=tile_src.TilesetName,
                                               start_level=start_level,
                                               longitude=longitude,
                                               latitude=latitude) if diagram is None else diagram
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/tile_worker.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/tile_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 For example, see osm_tiles.py.
 """
 import queue
 from urllib import request
 from collections.abc import Callable
 from PySide6.QtGui import QPixmap
 from PySide6.QtCore import QThread
-from GridCal.Gui.MapWidget.logger import log
+from GridCal.Gui.Diagrams.MapWidget.logger import log
 
 
 class TileWorker(QThread):
     """Thread class that gets request from queue, loads tile, calls callback."""
 
     def __init__(self,
                  id_num: int,
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/tiles.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,19 @@
 import math
 import traceback
 import urllib
 from urllib import request
 from urllib.error import HTTPError
 import queue
 from PySide6.QtGui import QPixmap, QColor
-# from PySide6 import QtG
 from typing import List
 from collections.abc import Callable
-from GridCal.Gui.MapWidget.Tiles.base_tiles import BaseTiles
-import GridCal.Gui.MapWidget.Tiles.default_tile_data as std
-from GridCal.Gui.MapWidget.Tiles.tile_worker import TileWorker
-from GridCal.Gui.MapWidget.logger import log
+from GridCal.Gui.Diagrams.MapWidget.Tiles.base_tiles import BaseTiles
+from GridCal.Gui.Diagrams.MapWidget.Tiles.tile_worker import TileWorker
+from GridCal.Gui.Diagrams.MapWidget.logger import log
 
 # # set how old disk-cache tiles can be before we re-request them from the
 # # server.  this is the number of days old a tile is before we re-request.
 # # if 'None', never re-request tiles after first satisfied request.
 # RefreshTilesAfterDays = 60
 
 # define the error messages for various failures
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/base_tiles.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/base_tiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 import os
 import math
 from typing import Tuple, Union, List
 from collections.abc import Callable
 from PySide6.QtGui import QPixmap
-from GridCal.Gui.MapWidget.Tiles.tiles_cache import TilesCache
+from GridCal.Gui.Diagrams.MapWidget.Tiles.tiles_cache import TilesCache
 
 
 class BaseTiles(object):
     """A base tile object to source local tiles for pySlip."""
 
     def __init__(self,
                  levels: List[int],
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/tiles_cache.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/tiles_cache.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 For example, see gmt_local.py (local tiles) and osm_tiles.py
 (internet tiles).
 """
 
 import os
 from typing import Tuple
 from PySide6.QtGui import QPixmap
-import GridCal.Gui.MapWidget.Tiles.pycacheback as pycacheback
+import GridCal.Gui.Diagrams.MapWidget.Tiles.pycacheback as pycacheback
 
 
 class TilesCache(pycacheback.PyCacheBack):
     """Cache for local or internet tiles.
 
     Instance variables we use from pyCacheBack:
         self._tiles_dir  path to the on-disk cache directory
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/pycacheback.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/pycacheback.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Tiles/default_tile_data.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Tiles/default_tile_data.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Schema/Nodes.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Schema/Nodes.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Schema/Connector.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Schema/Connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import numpy as np
 from typing import Union, TYPE_CHECKING
 from PySide6 import QtWidgets
 from PySide6.QtCore import Qt, QPoint, QRectF, QRect
 from PySide6.QtGui import QPen, QCursor, QIcon, QPixmap, QBrush, QColor
 from PySide6.QtWidgets import QGraphicsScene, QGraphicsLineItem
 
-from GridCal.Gui.MapWidget.Schema.Nodes import NodeGraphicItem
+from GridCal.Gui.Diagrams.MapWidget.Schema.Nodes import NodeGraphicItem
 
 
 class Connector(QGraphicsLineItem):
     def __init__(self, parent: QGraphicsScene, first: NodeGraphicItem, second: NodeGraphicItem):
         super().__init__()
         self.Parent = parent
         self.First = first
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Schema/SchemaManager.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Schema/SchemaManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 
-from GridCal.Gui.MapWidget.Schema.Nodes import NodeGraphicItem
-from GridCal.Gui.MapWidget.Schema.Connector import Connector
+from GridCal.Gui.Diagrams.MapWidget.Schema.Nodes import NodeGraphicItem
+from GridCal.Gui.Diagrams.MapWidget.Schema.Connector import Connector
 from GridCalEngine.Devices import MultiCircuit
 
 
 class schemaManager:
     def __init__(self, scene):
         self.disableMove = False
         self.Scene = scene
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/point_layer.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/point_layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from typing import List, Union, Tuple, Dict
 from collections.abc import Callable
-from GridCal.Gui.MapWidget.Layers.place import Place
-from GridCal.Gui.MapWidget.Layers.layer_types import LayerType
+from GridCal.Gui.Diagrams.MapWidget.Layers.place import Place
+from GridCal.Gui.Diagrams.MapWidget.Layers.layer_types import LayerType
 
 
 class PointData:
     """
     PointData
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/image_layer.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/image_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Tuple, Dict
 from collections.abc import Callable
-from GridCal.Gui.MapWidget.Layers.place import Place
-from GridCal.Gui.MapWidget.Layers.layer_types import LayerType
+from GridCal.Gui.Diagrams.MapWidget.Layers.place import Place
+from GridCal.Gui.Diagrams.MapWidget.Layers.layer_types import LayerType
 from PySide6.QtGui import QPixmap
 
 
 class ImageData:
     """
     PolylineDataPoint
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/polyline_layer.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/polyline_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from typing import List, Tuple, Dict
 from collections.abc import Callable
-from GridCal.Gui.MapWidget.Layers.place import Place
-from GridCal.Gui.MapWidget.Layers.layer_types import LayerType
+from GridCal.Gui.Diagrams.MapWidget.Layers.place import Place
+from GridCal.Gui.Diagrams.MapWidget.Layers.layer_types import LayerType
 
 
 class PolylineData:
     """
     PolylineDataPoint
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/text_layer.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/text_layer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from typing import List, Tuple, Dict
 from collections.abc import Callable
-from GridCal.Gui.MapWidget.Layers.place import Place
-from GridCal.Gui.MapWidget.Layers.layer_types import LayerType
+from GridCal.Gui.Diagrams.MapWidget.Layers.place import Place
+from GridCal.Gui.Diagrams.MapWidget.Layers.layer_types import LayerType
 
 
 class TextData:
     """
     PolylineDataPoint
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/Layers/polygon_layer.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/Layers/polygon_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from typing import List, Union, Tuple, Dict
 from collections.abc import Callable
-from GridCal.Gui.MapWidget.Layers.place import Place
-from GridCal.Gui.MapWidget.Layers.layer_types import LayerType
+from GridCal.Gui.Diagrams.MapWidget.Layers.place import Place
+from GridCal.Gui.Diagrams.MapWidget.Layers.layer_types import LayerType
 
 
 class PolygonData:
     """
     PolylineDataPoint
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/open_street_map.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/open_street_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A tile source that serves OpenStreetMap tiles from server(s).
 """
 
 import math
 from typing import Tuple
-from GridCal.Gui.MapWidget.Tiles.tiles import Tiles
+from GridCal.Gui.Diagrams.MapWidget.Tiles.tiles import Tiles
 
 
 class OsmTiles(Tiles):
     """An object to source server tiles for pySlipQt."""
 
     def __init__(self, tiles_dir='open_street_map_tiles', http_proxy=None):
         """Override the base class for these tiles.
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/mapbox.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A tile source that serves OpenStreetMap tiles from the internet.
 """
 
 import math
 from typing import Tuple
-from GridCal.Gui.MapWidget.Tiles.tiles import Tiles
+from GridCal.Gui.Diagrams.MapWidget.Tiles.tiles import Tiles
 
 
 class MapboxTiles(Tiles):
     """An object to source internet tiles for pySlip."""
 
     def __init__(self, tiles_dir='modest_maps_tiles', http_proxy=None):
         """Override the base class for these tiles.
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/cartodb.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/cartodb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A tile source that serves OpenStreetMap tiles from server(s).
 """
 
 import math
 from typing import Tuple
-from GridCal.Gui.MapWidget.Tiles.tiles import Tiles
+from GridCal.Gui.Diagrams.MapWidget.Tiles.tiles import Tiles
 
 
 class CartoDbTiles(Tiles):
     """An object to source server tiles for pySlipQt."""
 
     def __init__(self, tiles_dir='open_street_map_tiles', http_proxy=None, tile_servers=None):
         """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/mapquest.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/mapquest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A tile source that serves MapQuest tiles from the internet.
 """
 
 import math
 from typing import Tuple
-from GridCal.Gui.MapWidget.Tiles.tiles import Tiles
+from GridCal.Gui.Diagrams.MapWidget.Tiles.tiles import Tiles
 
 
 class MapquestTiles(Tiles):
     """An object to source internet tiles for pySlip."""
 
     def __init__(self, tiles_dir='mapquest_tiles', http_proxy=None):
         """Override the base class for these tiles.
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/stamen_transport.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Map tiles by Stamen Design, under CC BY 3.0. Data by OpenStreetMap, under CC BY SA.
 (See README.rst)
 """
 
 import math
 from typing import Tuple
-from GridCal.Gui.MapWidget.Tiles.tiles import Tiles
+from GridCal.Gui.Diagrams.MapWidget.Tiles.tiles import Tiles
 
 
 class StamenTransportTiles(Tiles):
     """An object to source internet tiles for pySlip."""
 
     def __init__(self, tiles_dir='stamen_transport_tiles', http_proxy=None):
         """Override the base class for these tiles.
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/stamen_watercolor.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_watercolor.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A tile source that serves Stamen Watercolor tiles from the internet.
 
 Map tiles by Stamen Design, under CC BY 3.0. Data by OpenStreetMap, under ODbL.
 """
 
 import math
 from typing import Tuple
-from GridCal.Gui.MapWidget.Tiles.tiles import Tiles
+from GridCal.Gui.Diagrams.MapWidget.Tiles.tiles import Tiles
 
 
 class StamenWatercolorTiles(Tiles):
     """An object to source internet tiles for pySlip."""
 
     def __init__(self, tiles_dir='stamen_watercolor_tiles', http_proxy=None):
         """Override the base class for these tiles.
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/blue_marble.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/blue_marble.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 A tile source that serves BlueMarble tiles from the internet.
 """
 
 import math
 from typing import Tuple
-import GridCal.Gui.MapWidget.Tiles.tiles as tiles_net
+import GridCal.Gui.Diagrams.MapWidget.Tiles.tiles as tiles_net
 
 
 class BlueMarbleTiles(tiles_net.Tiles):
     """
     An object to source internet tiles for pySlip.
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/stamen_toner.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/stamen_toner.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A tile source that serves Stamen Toner tiles from the internet.
 
 Map tiles by Stamen Design, under CC BY 3.0. Data by OpenStreetMap, under ODbL.
 """
 
 import math
 from typing import Tuple
-from GridCal.Gui.MapWidget.Tiles.tiles import Tiles
+from GridCal.Gui.Diagrams.MapWidget.Tiles.tiles import Tiles
 
 
 class StamenTonerTiles(Tiles):
     """An object to source internet tiles for pySlip."""
 
     def __init__(self, tiles_dir='stamen_toner_tiles', http_proxy=None):
         """Override the base class for these tiles.
```

### Comparing `GridCal-5.1.0/GridCal/Gui/MapWidget/TileProviders/gmt_local.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/MapWidget/TileProviders/gmt_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 A tile source that serves pre-generated GMT tiles from the local filesystem.
 """
 
 import os
 import pickle
 from typing import Tuple
-from GridCal.Gui.MapWidget.Tiles.base_tiles import BaseTiles
+from GridCal.Gui.Diagrams.MapWidget.Tiles.base_tiles import BaseTiles
 
 
 class GmtLocalTiles(BaseTiles):
     """An object to source GMT tiles for the widget."""
 
     TilesetName = 'GMT local tiles'
     TilesetShortName = 'GMT tiles'
```

### Comparing `GridCal-5.1.0/GridCal/Gui/RosetaExplorer/MainWindow.py` & `GridCal-5.1.1/GridCal/Gui/RosetaExplorer/MainWindow.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/RosetaExplorer/update_gui_file.py` & `GridCal-5.1.1/GridCal/Gui/RosetaExplorer/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/RosetaExplorer/RosetaExplorer.py` & `GridCal-5.1.1/GridCal/Gui/RosetaExplorer/RosetaExplorer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/RosetaExplorer/ConsoleWidget.py` & `GridCal-5.1.1/GridCal/Gui/RosetaExplorer/ConsoleWidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/RosetaExplorer/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/RosetaExplorer/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/LoadDesigner/load_designer.py` & `GridCal-5.1.1/GridCal/Gui/LoadDesigner/load_designer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/LoadDesigner/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/LoadDesigner/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/LoadDesigner/load_designer_ui.py` & `GridCal-5.1.1/GridCal/Gui/LoadDesigner/load_designer_ui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py` & `GridCal-5.1.1/GridCal/Gui/WindPowerWizard/wind_power_wizzard.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/WindPowerWizard/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/WindPowerWizard/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/WindPowerWizard/gui.py` & `GridCal-5.1.1/GridCal/Gui/WindPowerWizard/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/SystemScaler/system_scaler.py` & `GridCal-5.1.1/GridCal/Gui/SystemScaler/system_scaler.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/SystemScaler/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/SystemScaler/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/SystemScaler/system_scaler_ui.py` & `GridCal-5.1.1/GridCal/Gui/SystemScaler/system_scaler_ui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/TreeModelViewer/MainWindow.py` & `GridCal-5.1.1/GridCal/Gui/TreeModelViewer/MainWindow.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/TreeModelViewer/update_gui_file.py` & `GridCal-5.1.1/GridCal/Gui/TreeModelViewer/update_gui_file.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/TreeModelViewer/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/TreeModelViewer/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/TreeModelViewer/TreeModelViewer.py` & `GridCal-5.1.1/GridCal/Gui/TreeModelViewer/TreeModelViewer.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/matplotlibwidget.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/matplotlibwidget.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/terminal_item.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/terminal_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import Union, Any, TYPE_CHECKING, Callable, Dict
 from PySide6.QtCore import Qt, QPointF, QRectF, QRect
 from PySide6.QtGui import QPen, QCursor
 from PySide6.QtWidgets import (QGraphicsRectItem, QGraphicsItem, QGraphicsEllipseItem, QGraphicsSceneMouseEvent)
 
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
-    from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
-    from GridCal.Gui.BusBranchEditorWidget.Branches.transformer3w_graphics import Transformer3WGraphicItem
-    from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import BusGraphicItem
-    from GridCal.Gui.BusBranchEditorWidget.Fluid.fluid_node_graphics import FluidNodeGraphicItem
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.transformer3w_graphics import Transformer3WGraphicItem
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.Substation.bus_graphics import BusGraphicItem
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.Fluid.fluid_node_graphics import FluidNodeGraphicItem
 
 
 class TerminalItem(QGraphicsRectItem):
     """
     Represents a connection point to a subsystem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/bus_branch_editor_widget.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/bus_branch_editor_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,30 +54,31 @@
 from GridCalEngine.Simulations.driver_types import SimulationTypes
 from GridCalEngine.Simulations.driver_template import DriverTemplate
 from GridCalEngine.Devices.Diagrams.bus_branch_diagram import BusBranchDiagram
 from GridCalEngine.Devices.Diagrams.graphic_location import GraphicLocation
 from GridCalEngine.basic_structures import Vec, CxVec, IntVec, Logger
 from GridCalEngine.Devices.types import BRANCH_TYPES
 
-from GridCal.Gui.BusBranchEditorWidget.terminal_item import TerminalItem
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import BusGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Fluid.fluid_node_graphics import FluidNodeGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Fluid.fluid_path_graphics import FluidPathGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics import LineGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.winding_graphics import WindingGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.dc_line_graphics import DcLineGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.transformer2w_graphics import TransformerGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.hvdc_graphics import HvdcGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.vsc_graphics import VscGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.upfc_graphics import UpfcGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.series_reactance_graphics import SeriesReactanceGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.transformer3w_graphics import Transformer3WGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Injections.generator_graphics import GeneratorGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE
+from GridCal.Gui.Diagrams.graphics_manager import GraphicsManager
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Substation.bus_graphics import BusGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Fluid.fluid_node_graphics import FluidNodeGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Fluid.fluid_path_graphics import FluidPathGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics import LineGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.winding_graphics import WindingGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.dc_line_graphics import DcLineGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.transformer2w_graphics import TransformerGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.hvdc_graphics import HvdcGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.vsc_graphics import VscGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.upfc_graphics import UpfcGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.series_reactance_graphics import SeriesReactanceGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.transformer3w_graphics import Transformer3WGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.generator_graphics import GeneratorGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE
 from GridCal.Gui.GeneralDialogues import InputNumberDialogue
 import GridCal.Gui.Visualization.visualization as viz
 import GridCal.Gui.Visualization.palettes as palettes
 from GridCal.Gui.GuiFunctions import ObjectsModel, add_menu_entry
 from GridCal.Gui.messages import info_msg, error_msg, warning_msg, yes_no_question
 from matplotlib import pyplot as plt
 
@@ -95,31 +96,14 @@
   - .diagram {BusBranchDiagram} records the objects and their position to load and save diagrams
 
 
 The graphic objects need to call the API objects and functions inside the MultiCircuit instance.
 To do this the graphic objects call "parent.circuit.<function or object>"
 '''
 
-ALL_BUS_BRACH_GRAPHICS = Union[
-    BusGraphicItem,
-    FluidNodeGraphicItem,
-    FluidPathGraphicItem,
-    LineGraphicItem,
-    WindingGraphicItem,
-    DcLineGraphicItem,
-    TransformerGraphicItem,
-    HvdcGraphicItem,
-    VscGraphicItem,
-    UpfcGraphicItem,
-    SeriesReactanceGraphicItem,
-    LineGraphicTemplateItem,
-    Transformer3WGraphicItem,
-    GeneratorGraphicItem
-]
-
 
 class BusBranchLibraryModel(QStandardItemModel):
     """
     Items model to host the draggable icons
     This is the list of draggable items
     """
 
@@ -128,37 +112,32 @@
         Items model to host the draggable icons
         @param parent:
         """
         QStandardItemModel.__init__(self, parent)
 
         self.setColumnCount(1)
 
-        # add bus to the drag&drop
-        bus_icon = QIcon()
-        bus_icon.addPixmap(QPixmap(":/Icons/icons/bus_icon.svg"))
+        def add(name: str, icon_name: str):
+            _icon = QIcon()
+            _icon.addPixmap(QPixmap(f":/Icons/icons/{icon_name}.svg"))
+            _item = QStandardItem(_icon, name)
+            _item.setToolTip("Drag & drop this into the schematic")
+            self.appendRow(_item)
+
         self.bus_name = "Bus"
-        item = QStandardItem(bus_icon, self.bus_name)
-        item.setToolTip("Drag & drop this into the schematic")
-        self.appendRow(item)
-
-        # add transformer3w to the drag&drop
-        t3w_icon = QIcon()
-        t3w_icon.addPixmap(QPixmap(":/Icons/icons/transformer3w.svg"))
         self.transformer3w_name = "3W-Transformer"
-        item = QStandardItem(t3w_icon, self.transformer3w_name)
-        item.setToolTip("Drag & drop this into the schematic")
-        self.appendRow(item)
-
-        # add fluid-node to the drag&drop
-        dam_icon = QIcon()
-        dam_icon.addPixmap(QPixmap(":/Icons/icons/dam.svg"))
         self.fluid_node_name = "Fluid-node"
-        item = QStandardItem(dam_icon, self.fluid_node_name)
-        item.setToolTip("Drag & drop this into the schematic")
-        self.appendRow(item)
+        self.cn_name = "Connectivity node"
+        self.bb_name = "Bus bar"
+
+        add(name=self.bus_name, icon_name="bus_icon")
+        add(name=self.transformer3w_name, icon_name="transformer3w")
+        add(name=self.fluid_node_name, icon_name="dam")
+        # add(name=self.cn_name, icon_name="cn_icon")
+        # add(name=self.bb_name, icon_name="bus_bar_icon")
 
     @staticmethod
     def to_bytes_array(val: str) -> QByteArray:
         """
         Convert string to QByteArray
         :param val: string
         :return: QByteArray
@@ -185,14 +164,28 @@
     def get_fluid_node_mime_data(self) -> QByteArray:
         """
 
         :return:
         """
         return self.to_bytes_array(self.fluid_node_name)
 
+    def get_connectivity_node_mime_data(self) -> QByteArray:
+        """
+
+        :return:
+        """
+        return self.to_bytes_array(self.cn_name)
+
+    def get_bus_bar_mime_data(self) -> QByteArray:
+        """
+
+        :return:
+        """
+        return self.to_bytes_array(self.bb_name)
+
     def mimeTypes(self) -> List[str]:
         """
 
         @return:
         """
         return ['component/name']
 
@@ -444,107 +437,14 @@
     """
     graphic_obj = bus_dict.get(idtag_, None)
     if graphic_obj is None:
         graphic_obj = fluid_node_dict.get(idtag_, None)
     return graphic_obj
 
 
-class GraphicsManager:
-    """
-    Class to handle the correspondance between graphics and database devices
-    """
-
-    def __init__(self):
-        # this is a dictionary that groups by 2 levels:
-        # first by DeviceType
-        # second idtag -> GraphicItem
-        self.graphic_dict: Dict[DeviceType, Dict[str, ALL_BUS_BRACH_GRAPHICS]] = dict()
-
-    def add_device(self, elm: ALL_DEV_TYPES, graphic: ALL_BUS_BRACH_GRAPHICS) -> None:
-        """
-        Add the graphic of a device
-        :param elm: Any database device
-        :param graphic: Corresponding graphic
-        """
-        if graphic is not None:  # it makes no sense to add a None graphic
-
-            elm_dict: Dict[str, ALL_BUS_BRACH_GRAPHICS] = self.graphic_dict.get(elm.device_type, None)
-
-            if elm_dict is None:
-                self.graphic_dict[elm.device_type] = {elm.idtag: graphic}
-            else:
-                graphic_0 = elm_dict.get(elm.idtag, None)  # try to get the existing element
-                if graphic_0 is None:
-                    elm_dict[elm.idtag] = graphic
-                else:
-                    if graphic_0 != graphic:
-                        warn(f"Replacing {graphic} with {graphic}, this could be a sign of an idtag bug")
-                    elm_dict[elm.idtag] = graphic
-        else:
-            raise ValueError(f"Trying to set a None graphic object for {elm}")
-
-    def delete_device(self, device: ALL_DEV_TYPES) -> Union[ALL_BUS_BRACH_GRAPHICS, None]:
-        """
-        Delete device from the registry and return the object if it exists
-        :param device: Any database device
-        :return: Corresponding graphic or None
-        """
-        if device is not None:
-            # check if the category exists ...
-            elm_dict = self.graphic_dict.get(device.device_type, None)
-
-            if elm_dict is not None:
-                # the category does exist, delete from it
-                graphic = elm_dict.get(device.idtag, None)
-
-                if graphic:
-                    del elm_dict[device.idtag]
-                    return graphic
-
-            else:
-                # not found so we're ok
-                return None
-        else:
-            return None
-
-    def query(self, elm: ALL_DEV_TYPES) -> Union[None, ALL_BUS_BRACH_GRAPHICS]:
-        """
-        Query the graphic of a database element
-        :param elm: Any database element
-        :return: Corresponding graphic
-        """
-        elm_dict: Dict[str, ALL_BUS_BRACH_GRAPHICS] = self.graphic_dict.get(elm.device_type, None)
-
-        if elm_dict is None:
-            return None
-        else:
-            return elm_dict.get(elm.idtag, None)
-
-    def get_device_type_list(self, device_type: DeviceType) -> List[ALL_BUS_BRACH_GRAPHICS]:
-        """
-        Get the list of graphics of a device type
-        :param device_type: DeviceType
-        :return: List[ALL_BUS_BRACH_GRAPHICS]
-        """
-        elm_dict: Dict[str, ALL_BUS_BRACH_GRAPHICS] = self.graphic_dict.get(device_type, None)
-
-        if elm_dict is None:
-            return list()
-        else:
-            return [graphic for idtag, graphic in elm_dict.items()]
-
-    def get_device_type_dict(self, device_type: DeviceType) -> Dict[str, ALL_BUS_BRACH_GRAPHICS]:
-        """
-        Get the list of graphics of a device type
-        :param device_type: DeviceType
-        :return: Dict[str, ALL_BUS_BRACH_GRAPHICS]
-        """
-        return self.graphic_dict.get(device_type, dict())
-
-
 class BusBranchEditorWidget(QSplitter):
     """
     BusBranchEditorWidget
     This is the bus-branch editor
     """
 
     def __init__(self,
@@ -702,23 +602,20 @@
         """
         Create an element
         @param event:
         @return:
         """
         if event.mimeData().hasFormat('component/name'):
             obj_type = event.mimeData().data('component/name')
-            bus_data = self.library_model.get_bus_mime_data()
-            tr3w_data = self.library_model.get_3w_transformer_mime_data()
-            fluid_node_data = self.library_model.get_fluid_node_mime_data()
 
             point0 = self.editor_graphics_view.mapToScene(event.position().x(), event.position().y())
             x0 = point0.x()
             y0 = point0.y()
 
-            if bus_data == obj_type:
+            if obj_type == self.library_model.get_bus_mime_data():
                 obj = Bus(name=f'Bus {len(self.circuit.get_buses())}',
                           vnom=self.default_bus_voltage)
 
                 graphic_object = BusGraphicItem(editor=self,
                                                 bus=obj,
                                                 x=x0,
                                                 y=y0,
@@ -735,15 +632,15 @@
                                             x=x0,
                                             y=y0,
                                             w=graphic_object.w,
                                             h=graphic_object.h,
                                             r=0,
                                             graphic_object=graphic_object)
 
-            elif tr3w_data == obj_type:
+            elif obj_type == self.library_model.get_3w_transformer_mime_data():
                 obj = Transformer3W(name=f"Transformer 3W {len(self.circuit.transformers3w)}")
                 graphic_object = self.create_transformer_3w_graphics(elm=obj, x=x0, y=y0)
                 self.add_to_scene(graphic_object=graphic_object)
 
                 # weird but it's the only way to have graphical-API communication
                 self.circuit.add_transformer3w(obj)
 
@@ -752,32 +649,39 @@
                                             x=x0,
                                             y=y0,
                                             w=graphic_object.w,
                                             h=graphic_object.h,
                                             r=0,
                                             graphic_object=graphic_object)
 
-            elif fluid_node_data == obj_type:
+            elif obj_type == self.library_model.get_fluid_node_mime_data():
                 obj = FluidNode(name=f"Fluid node {len(self.circuit.fluid_nodes)}")
 
                 graphic_object = self.create_fluid_node_graphics(node=obj, x=x0, y=y0, h=20, w=80)
+
                 self.add_to_scene(graphic_object=graphic_object)
 
                 # weird but it's the only way to have graphical-API communication
                 self.circuit.add_fluid_node(obj)
 
                 # add to the diagram list
                 self.update_diagram_element(device=obj,
                                             x=x0,
                                             y=y0,
                                             w=graphic_object.w,
                                             h=graphic_object.h,
                                             r=0,
                                             graphic_object=graphic_object)
 
+            elif obj_type == self.library_model.get_connectivity_node_mime_data():
+                pass
+
+            elif obj_type == self.library_model.get_bus_bar_mime_data():
+                pass
+
     def graphicsWheelEvent(self, event: QWheelEvent) -> None:
         """
         Zoom
         @param event:
         @return:
         """
         self.editor_graphics_view.setTransformationAnchor(QGraphicsView.ViewportAnchor.AnchorUnderMouse)
@@ -2975,14 +2879,15 @@
 
         bus_types = ['', 'PQ', 'PV', 'Slack', 'None', 'Storage', 'P', 'PQV']
         max_flow = 1
 
         if len(buses) == len(vnorm):
             for i, bus in enumerate(buses):
 
+                # try to find the diagram object of the DB object
                 graphic_object = self.graphics_manager.query(bus)
 
                 if graphic_object:
 
                     if bus_active[i]:
                         a = 255
                         if cmap == palettes.Colormaps.Green2Red:
@@ -2999,43 +2904,30 @@
                             r *= 255
                             g *= 255
                             b *= 255
                             a *= 255
 
                         graphic_object.set_tile_color(QColor(r, g, b, a))
 
-                        tooltip = str(i) + ': ' + bus.name
-                        if types is not None:
-                            tooltip += ': ' + bus_types[types[i]]
-                        tooltip += '\n'
-
-                        # tooltip += "%-10s %10.4f < %10.4fº [p.u.]\n" % ("V", vabs[i], vang[i])
-                        # tooltip += "%-10s %10.4f < %10.4fº [kV]\n" % ("V", vabs[i] * bus.Vnom, vang[i])
-                        #
-                        # if Sbus is not None:
-                        #     tooltip += "%-10s %10.4f [MW]\n" % ("P", Sbus[i].real)
-                        #     tooltip += "%-10s %10.4f [MVAr]\n" % ("Q", Sbus[i].imag)
-
-                        graphic_object.setToolTip(tooltip)
                         graphic_object.set_values(i=i,
                                                   Vm=vabs[i],
                                                   Va=vang[i],
                                                   P=Sbus[i].real if Sbus is not None else None,
                                                   Q=Sbus[i].imag if Sbus is not None else None,
                                                   tpe=bus_types[types[i]] if types is not None else None)
 
                         if use_flow_based_width:
-                            # h = int(np.floor(min_bus_width + Pnorm[i] * (max_bus_width - min_bus_width)))
                             graphic_object.change_size(w=graphic_object.w)
 
                     else:
                         graphic_object.set_tile_color(Qt.gray)
 
                 else:
-                    print("Bus {0} {1} has no graphic object!!".format(bus.name, bus.idtag))
+                    # No graphic object found
+                    pass
         else:
             error_msg("Bus results length differs from the number of Bus results. \n"
                       "Did you change the number of devices? If so, re-run the simulation.")
             return
 
         # color Branches
         if Sf is not None:
@@ -3053,14 +2945,15 @@
                     Sfnorm = Sfabs / max_flow
                 else:
                     Sfnorm = Sfabs
 
                 if len(branches) == len(Sf):
                     for i, branch in enumerate(branches):
 
+                        # try to find the diagram object of the DB object
                         graphic_object = self.graphics_manager.query(branch)
 
                         if graphic_object:
 
                             if br_active[i]:
 
                                 if use_flow_based_width:
@@ -3129,28 +3022,29 @@
                                         St=St[i] if St is not None else None)
                             else:
                                 w = graphic_object.pen_width
                                 style = Qt.DashLine
                                 color = Qt.gray
                                 graphic_object.set_pen(QPen(color, w, style))
                         else:
-                            print("Branch {0} {1} has no graphic object!!".format(branch.name, branch.idtag))
-
+                            # No diagram object
+                            pass
                 else:
                     error_msg("Branch results length differs from the number of branch results. \n"
                               "Did you change the numbe rof devices? If so, re-run the simulation.")
                     return
 
         if hvdc_Pf is not None:
 
             hvdc_sending_power_norm = np.abs(hvdc_Pf) / (max_flow + 1e-20)
 
             if len(hvdc_lines) == len(hvdc_Pf):
                 for i, elm in enumerate(hvdc_lines):
 
+                    # try to find the diagram object of the DB object
                     graphic_object = self.graphics_manager.query(elm)
 
                     if graphic_object:
 
                         if hvdc_active[i]:
 
                             if use_flow_based_width:
@@ -3203,15 +3097,16 @@
                             graphic_object.set_colour(color, w, style)
                         else:
                             w = graphic_object.pen_width
                             style = Qt.DashLine
                             color = Qt.gray
                             graphic_object.set_pen(QPen(color, w, style))
                     else:
-                        print("HVDC line {0} {1} has no graphic object!!".format(elm.name, elm.idtag))
+                        # No diagram object
+                        pass
             else:
                 error_msg("HVDC results length differs from the number of HVDC results. \n"
                           "Did you change the numbe rof devices? If so, re-run the simulation.")
 
     def get_selected(self) -> List[Tuple[ALL_DEV_TYPES, QGraphicsItem]]:
         """
         Get selection
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Fluid/fluid_turbine_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Fluid/fluid_turbine_graphics.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,34 +12,31 @@
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
-from PySide6.QtCore import QPointF
 from PySide6.QtGui import QPen, QIcon, QPixmap
 from PySide6.QtWidgets import (QMenu, QGraphicsTextItem, QGraphicsSceneMouseEvent)
-from GridCalEngine.enumerations import DeviceType
 from GridCalEngine.Devices.Fluid.fluid_turbine import FluidTurbine
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
-from GridCal.Gui.GuiFunctions import ObjectsModel
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class FluidTurbineGraphicItem(InjectionTemplateGraphicItem):
     """
     FluidTurbineGraphicItem
     """
 
-    def __init__(self, parent, api_obj: FluidTurbine, editor: "BusBranchEditorWidget"):
+    def __init__(self, parent, api_obj: FluidTurbine, editor: BusBranchEditorWidget):
         """
 
         :param parent:
         :param api_obj:
         :param editor:
         """
         InjectionTemplateGraphicItem.__init__(self,
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Fluid/fluid_pump_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Fluid/fluid_pump_graphics.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtCore import QPointF
 from PySide6.QtGui import QPen, QIcon, QPixmap
 from PySide6.QtWidgets import (QMenu, QGraphicsTextItem)
 from GridCalEngine.Devices.Fluid.fluid_pump import FluidPump
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class FluidPumpGraphicItem(InjectionTemplateGraphicItem):
     """
     FluidPumpGraphicItem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Fluid/fluid_path_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Fluid/fluid_path_graphics.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,25 +15,23 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import Union, TYPE_CHECKING
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QPen, QIcon, QPixmap, QColor
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.GeneralDialogues import InputNumberDialogue
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import TerminalItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_editor import LineEditor
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import GenericDBWidget, ACTIVE
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 from GridCalEngine.Devices.Fluid.fluid_path import FluidPath
 from GridCalEngine.enumerations import DeviceType
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget import BusBranchEditorWidget
 
 
 class FluidPathGraphicItem(LineGraphicTemplateItem):
     """
     LineGraphicItem
     """
 
@@ -49,14 +47,15 @@
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
         :param arrow_size:
         """
+        GenericDBWidget.__init__(self, parent=None, api_object=api_object, editor=editor, draw_labels=True)
         LineGraphicTemplateItem.__init__(self,
                                          from_port=from_port,
                                          to_port=to_port,
                                          editor=editor,
                                          width=width,
                                          api_object=api_object,
                                          arrow_size=arrow_size)
@@ -89,14 +88,15 @@
         if self.symbol is not None:
             self.symbol.set_colour(color, w, style)
 
     def recolour_mode(self):
         """
         Change the colour according to the system theme
         """
+        # super().recolour_mode()
         self.set_colour(self.color, self.width, self.style)
 
     def mouseDoubleClickEvent(self, event):
         """
         On double click, edit
         :param event:
         :return:
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Fluid/fluid_p2x_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Fluid/fluid_p2x_graphics.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtCore import QPointF
 from PySide6.QtGui import QPen, QIcon, QPixmap
 from PySide6.QtWidgets import (QMenu, QGraphicsTextItem)
 from GridCalEngine.Devices.Fluid.fluid_p2x import FluidP2x
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class FluidP2xGraphicItem(InjectionTemplateGraphicItem):
     """
     FluidP2xGraphicItem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Fluid/fluid_node_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Fluid/fluid_node_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,35 @@
 import numpy as np
 from typing import Union, TYPE_CHECKING, List, Dict
 from PySide6 import QtWidgets
 from PySide6.QtCore import Qt, QPoint
 from PySide6.QtGui import QPen, QCursor, QIcon, QPixmap, QBrush, QPainterPath, QFont
 from PySide6.QtWidgets import QMenu, QGraphicsRectItem, QGraphicsSceneMouseEvent, QGraphicsTextItem
 
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, FONT_SCALE
 from GridCalEngine.Devices.Fluid import FluidNode, FluidTurbine, FluidPump, FluidP2x
 from GridCalEngine.Devices.Substation.bus import Bus
-from GridCal.Gui.BusBranchEditorWidget.terminal_item import TerminalItem, HandleItem
-from GridCal.Gui.BusBranchEditorWidget.Fluid.fluid_turbine_graphics import FluidTurbineGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Fluid.fluid_pump_graphics import FluidPumpGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Fluid.fluid_p2x_graphics import FluidP2xGraphicItem
-from GridCal.Gui.messages import yes_no_question
 from GridCalEngine.enumerations import DeviceType, FaultType
 from GridCalEngine.Devices.Parents.editable_device import EditableDevice
+from GridCalEngine.Devices.types import FLUID_TYPES
+
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, FONT_SCALE, GenericDBWidget
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem, HandleItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Fluid.fluid_turbine_graphics import FluidTurbineGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Fluid.fluid_pump_graphics import FluidPumpGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Fluid.fluid_p2x_graphics import FluidP2xGraphicItem
+from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget import BusBranchEditorWidget
 
 
 class RoundedRect(QtWidgets.QGraphicsRectItem):
+    """
+    Rounded rectangle
+    """
     def __init__(self, x, y, width, height, radius, parent):
         super().__init__(x, y, width, height, parent=parent)
         self.radius = radius
 
     def paint(self, painter, option, widget):
         path = QPainterPath()
         path.addRoundedRect(self.rect(), self.radius, self.radius)
@@ -72,40 +77,37 @@
                                 self.rect().width(), inner_height)
         self.inner_rect.setPos(self.rect().x(), self.rect().y())
 
         # Update the label text
         self.label.setPlainText(f'{percentage}%')
 
 
-class FluidNodeGraphicItem(QtWidgets.QGraphicsRectItem):
+class FluidNodeGraphicItem(GenericDBWidget, QtWidgets.QGraphicsRectItem):
     """
       Represents a block in the diagram
       Has an x and y and width and height
       width and height can only be adjusted with a tip in the lower right corner.
 
       - in and output ports
       - parameters
       - description
     """
 
     def __init__(self, editor: BusBranchEditorWidget, fluid_node: FluidNode,
                  parent=None, index=0, h: int = 20, w: int = 80, x: int = 0, y: int = 0):
 
-        super(FluidNodeGraphicItem, self).__init__(parent)
+        GenericDBWidget.__init__(self, parent=parent, api_object=fluid_node, editor=editor, draw_labels=True)
+        QtWidgets.QGraphicsRectItem.__init__(self, parent)
 
         self.min_w = 180.0
         self.min_h = 20.0
         self.offset = 10
         self.h = h if h >= self.min_h else self.min_h
         self.w = w if w >= self.min_w else self.min_w
 
-        self.api_object = fluid_node
-
-        self.editor: BusBranchEditorWidget = editor
-
         # loads, shunts, generators, etc...
         self.shunt_children = list()
 
         # Enabled for short circuit
         self.sc_enabled = [False, False, False, False]
         self.sc_type = FaultType.ph3
         self.pen_width = 4
@@ -300,15 +302,15 @@
         for elm in self.shunt_children:
             elm.setPos(x - elm.w / 2, y0)
             x += inc_x
 
         # Arrange line positions
         self._terminal.process_callbacks(self.pos() + self._terminal.pos())
 
-    def create_children_widgets(self, injections_by_tpe: Dict[DeviceType, List[EditableDevice]]):
+    def create_children_widgets(self, injections_by_tpe: Dict[DeviceType, List[FLUID_TYPES]]):
         """
         Create the icons of the elements that are attached to the API bus object
         Returns:
             Nothing
         """
         for tpe, dev_list in injections_by_tpe.items():
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/winding_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/winding_graphics.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
 from GridCal.Gui.messages import yes_no_question
 from GridCalEngine.Devices.Branches.winding import Winding
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget import BusBranchEditorWidget
 
 
 class WindingGraphicItem(LineGraphicTemplateItem):
 
     def __init__(self,
                  from_port: TerminalItem,
                  to_port: Union[TerminalItem, None],
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/line_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/line_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,23 +15,23 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING, Union
 from PySide6.QtCore import Qt, QRectF
 from PySide6.QtGui import QPen, QIcon, QPixmap, QBrush
 from PySide6.QtWidgets import QMenu, QGraphicsRectItem, QGraphicsSceneContextMenuEvent
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import TerminalItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_editor import LineEditor
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_editor import LineEditor
 from GridCal.Gui.messages import yes_no_question, warning_msg
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 from GridCalEngine.Devices.Branches.line import Line, SequenceLineType
 from GridCalEngine.enumerations import DeviceType
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget import BusBranchEditorWidget
 
 
 class LineGraphicItem(LineGraphicTemplateItem):
     """
     LineGraphicItem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/switch_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/series_reactance_graphics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 # GridCal
 # Copyright (C) 2015 - 2024 Santiago Peñate Vera
-#
+# 
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 3 of the License, or (at your option) any later version.
-#
+# 
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
-#
+# 
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING
 from PySide6.QtGui import QIcon, QPixmap
-from PySide6.QtWidgets import QMenu, QGraphicsScene
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import TerminalItem
-from GridCalEngine.Devices.Branches.switch import Switch
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from PySide6.QtWidgets import QMenu
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
+from GridCalEngine.Devices.Branches.series_reactance import SeriesReactance
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
-class SwitchGraphicItem(LineGraphicTemplateItem):
+class SeriesReactanceGraphicItem(LineGraphicTemplateItem):
 
-    def __init__(self, from_port: TerminalItem,
-                 to_port: Union[TerminalItem, None],
-                 editor: BusBranchEditorWidget,
-                 width=5,
-                 api_object: Switch = None):
+    def __init__(self, from_port: TerminalItem, to_port: TerminalItem,
+                 editor: BusBranchEditorWidget, width=5,
+                 api_object: SeriesReactance = None):
         """
 
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
@@ -52,29 +50,40 @@
         """
         Show context menu
         @param event:
         @return:
         """
         if self.api_object is not None:
             menu = QMenu()
-            menu.addSection("Line")
 
-            pe = menu.addAction('Active')
-            pe.setCheckable(True)
-            pe.setChecked(self.api_object.active)
+            pe = menu.addAction('Enable/Disable')
+            pe_icon = QIcon()
+            if self.api_object.active:
+                pe_icon.addPixmap(QPixmap(":/Icons/icons/uncheck_all.svg"))
+            else:
+                pe_icon.addPixmap(QPixmap(":/Icons/icons/check_all.svg"))
+            pe.setIcon(pe_icon)
             pe.triggered.connect(self.enable_disable_toggle)
 
             rabf = menu.addAction('Change bus')
             move_bus_icon = QIcon()
             move_bus_icon.addPixmap(QPixmap(":/Icons/icons/move_bus.svg"))
             rabf.setIcon(move_bus_icon)
             rabf.triggered.connect(self.change_bus)
 
             menu.addSeparator()
 
+            ra2 = menu.addAction('Delete')
+            del_icon = QIcon()
+            del_icon.addPixmap(QPixmap(":/Icons/icons/delete3.svg"))
+            ra2.setIcon(del_icon)
+            ra2.triggered.connect(self.remove)
+
+            menu.addSeparator()
+
             ra6 = menu.addAction('Plot profiles')
             plot_icon = QIcon()
             plot_icon.addPixmap(QPixmap(":/Icons/icons/plot.svg"))
             ra6.setIcon(plot_icon)
             ra6.triggered.connect(self.plot_profiles)
 
             ra4 = menu.addAction('Assign rate to profile')
@@ -85,18 +94,11 @@
 
             ra5 = menu.addAction('Assign active state to profile')
             ra5_icon = QIcon()
             ra5_icon.addPixmap(QPixmap(":/Icons/icons/assign_to_profile.svg"))
             ra5.setIcon(ra5_icon)
             ra5.triggered.connect(self.assign_status_to_profile)
 
-            # menu.addSeparator()
-
-            ra2 = menu.addAction('Delete')
-            del_icon = QIcon()
-            del_icon.addPixmap(QPixmap(":/Icons/icons/delete3.svg"))
-            ra2.setIcon(del_icon)
-            ra2.triggered.connect(self.remove)
 
             menu.exec_(event.screenPos())
         else:
             pass
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/series_reactance_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/hvdc_graphics.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,30 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import TerminalItem
-from GridCalEngine.Devices.Branches.series_reactance import SeriesReactance
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
+from GridCalEngine.Devices.Branches.hvdc_line import HvdcLine
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget import BusBranchEditorWidget
 
 
-class SeriesReactanceGraphicItem(LineGraphicTemplateItem):
+class HvdcGraphicItem(LineGraphicTemplateItem):
 
-    def __init__(self, from_port: TerminalItem, to_port: TerminalItem,
-                 editor: BusBranchEditorWidget, width=5,
-                 api_object: SeriesReactance = None):
+    def __init__(self,
+                 from_port: TerminalItem,
+                 to_port: TerminalItem,
+                 editor: BusBranchEditorWidget,
+                 width=5,
+                 api_object: HvdcLine = None):
         """
 
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
@@ -50,40 +53,32 @@
         """
         Show context menu
         @param event:
         @return:
         """
         if self.api_object is not None:
             menu = QMenu()
+            menu.addSection("HVDC line")
 
-            pe = menu.addAction('Enable/Disable')
-            pe_icon = QIcon()
-            if self.api_object.active:
-                pe_icon.addPixmap(QPixmap(":/Icons/icons/uncheck_all.svg"))
-            else:
-                pe_icon.addPixmap(QPixmap(":/Icons/icons/check_all.svg"))
-            pe.setIcon(pe_icon)
+            pe = menu.addAction('Active')
+            pe.setCheckable(True)
+            pe.setChecked(self.api_object.active)
             pe.triggered.connect(self.enable_disable_toggle)
 
+            # pe2 = menu.addAction('Convert to Multi-terminal')
+            # pe2.triggered.connect(self.convert_to_multi_terminal)
+
             rabf = menu.addAction('Change bus')
             move_bus_icon = QIcon()
             move_bus_icon.addPixmap(QPixmap(":/Icons/icons/move_bus.svg"))
             rabf.setIcon(move_bus_icon)
             rabf.triggered.connect(self.change_bus)
 
             menu.addSeparator()
 
-            ra2 = menu.addAction('Delete')
-            del_icon = QIcon()
-            del_icon.addPixmap(QPixmap(":/Icons/icons/delete3.svg"))
-            ra2.setIcon(del_icon)
-            ra2.triggered.connect(self.remove)
-
-            menu.addSeparator()
-
             ra6 = menu.addAction('Plot profiles')
             plot_icon = QIcon()
             plot_icon.addPixmap(QPixmap(":/Icons/icons/plot.svg"))
             ra6.setIcon(plot_icon)
             ra6.triggered.connect(self.plot_profiles)
 
             ra4 = menu.addAction('Assign rate to profile')
@@ -94,11 +89,31 @@
 
             ra5 = menu.addAction('Assign active state to profile')
             ra5_icon = QIcon()
             ra5_icon.addPixmap(QPixmap(":/Icons/icons/assign_to_profile.svg"))
             ra5.setIcon(ra5_icon)
             ra5.triggered.connect(self.assign_status_to_profile)
 
+            ra2 = menu.addAction('Delete')
+            del_icon = QIcon()
+            del_icon.addPixmap(QPixmap(":/Icons/icons/delete3.svg"))
+            ra2.setIcon(del_icon)
+            ra2.triggered.connect(self.remove)
 
             menu.exec_(event.screenPos())
         else:
             pass
+
+    def convert_to_multi_terminal(self):
+        """
+
+        """
+        pass
+
+    def plot_profiles(self):
+        """
+        Plot the time series profiles
+        @return:
+        """
+        # get the index of this object
+        i = self.editor.circuit.get_hvdc().index(self.api_object)
+        self.editor.plot_hvdc_branch(i, self.api_object)
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/dc_line_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/dc_line_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 import numpy as np
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu, QLabel, QDoubleSpinBox, QPushButton, QVBoxLayout, QComboBox, QDialog, QGraphicsScene
 from GridCal.Gui.GuiFunctions import get_list_model
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
 from GridCalEngine.Devices.Branches.line import SequenceLineType, OverheadLineType, UndergroundLineType
 from GridCalEngine.Devices.Branches.dc_line import DcLine
 from GridCalEngine.enumerations import DeviceType
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget import BusBranchEditorWidget
 
 
 class DcLineEditor(QDialog):
     """
     DcLineEditor
     """
     def __init__(self, branch: DcLine, Sbase=100, templates=None, current_template=None):
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/hvdc_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/switch_graphics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # GridCal
 # Copyright (C) 2015 - 2024 Santiago Peñate Vera
-# 
+#
 # This program is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 3 of the License, or (at your option) any later version.
-# 
+#
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
-# 
+#
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Union
 from PySide6.QtGui import QIcon, QPixmap
-from PySide6.QtWidgets import QMenu
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import TerminalItem
-from GridCalEngine.Devices.Branches.hvdc_line import HvdcLine
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from PySide6.QtWidgets import QMenu, QGraphicsScene
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
+from GridCalEngine.Devices.Branches.switch import Switch
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
-class HvdcGraphicItem(LineGraphicTemplateItem):
+class SwitchGraphicItem(LineGraphicTemplateItem):
 
-    def __init__(self,
-                 from_port: TerminalItem,
-                 to_port: TerminalItem,
+    def __init__(self, from_port: TerminalItem,
+                 to_port: Union[TerminalItem, None],
                  editor: BusBranchEditorWidget,
                  width=5,
-                 api_object: HvdcLine = None):
+                 api_object: Switch = None):
         """
 
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
@@ -53,24 +52,21 @@
         """
         Show context menu
         @param event:
         @return:
         """
         if self.api_object is not None:
             menu = QMenu()
-            menu.addSection("HVDC line")
+            menu.addSection("Line")
 
             pe = menu.addAction('Active')
             pe.setCheckable(True)
             pe.setChecked(self.api_object.active)
             pe.triggered.connect(self.enable_disable_toggle)
 
-            # pe2 = menu.addAction('Convert to Multi-terminal')
-            # pe2.triggered.connect(self.convert_to_multi_terminal)
-
             rabf = menu.addAction('Change bus')
             move_bus_icon = QIcon()
             move_bus_icon.addPixmap(QPixmap(":/Icons/icons/move_bus.svg"))
             rabf.setIcon(move_bus_icon)
             rabf.triggered.connect(self.change_bus)
 
             menu.addSeparator()
@@ -89,31 +85,18 @@
 
             ra5 = menu.addAction('Assign active state to profile')
             ra5_icon = QIcon()
             ra5_icon.addPixmap(QPixmap(":/Icons/icons/assign_to_profile.svg"))
             ra5.setIcon(ra5_icon)
             ra5.triggered.connect(self.assign_status_to_profile)
 
+            # menu.addSeparator()
+
             ra2 = menu.addAction('Delete')
             del_icon = QIcon()
             del_icon.addPixmap(QPixmap(":/Icons/icons/delete3.svg"))
             ra2.setIcon(del_icon)
             ra2.triggered.connect(self.remove)
 
             menu.exec_(event.screenPos())
         else:
             pass
-
-    def convert_to_multi_terminal(self):
-        """
-
-        """
-        pass
-
-    def plot_profiles(self):
-        """
-        Plot the time series profiles
-        @return:
-        """
-        # get the index of this object
-        i = self.editor.circuit.get_hvdc().index(self.api_object)
-        self.editor.plot_hvdc_branch(i, self.api_object)
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/upfc_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/upfc_graphics.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
 from GridCalEngine.Devices.Branches.upfc import UPFC
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class UpfcGraphicItem(LineGraphicTemplateItem):
 
     def __init__(self, from_port: TerminalItem, to_port: TerminalItem,
                  editor: BusBranchEditorWidget, width=5,
                  api_object: UPFC = None):
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/transformer2w_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/transformer2w_graphics.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.BusBranchEditorWidget.Branches.transformer_editor import (TransformerEditor,
-                                                                           reverse_transformer_short_circuit_study)
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.transformer_editor import (TransformerEditor,
+                                                                                    reverse_transformer_short_circuit_study)
 from GridCalEngine.Devices.Branches.transformer import Transformer2W, TransformerType
 from GridCalEngine.enumerations import DeviceType
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class TransformerGraphicItem(LineGraphicTemplateItem):
     """
     TransformerGraphicItem
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/line_editor.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/line_editor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/vsc_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/vsc_graphics.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtGui import QIcon, QPixmap
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import TerminalItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
 from GridCalEngine.Devices.Branches.vsc import VSC
-from GridCal.Gui.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.line_graphics_template import LineGraphicTemplateItem
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class VscGraphicItem(LineGraphicTemplateItem):
     """
     Graphics item for the VSC converter
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/transformer3w_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/transformer3w_graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,21 @@
 import numpy as np
 from typing import List, TYPE_CHECKING
 from PySide6.QtCore import Qt, QPoint, QPointF
 from PySide6.QtGui import QPen, QCursor, QColor, QIcon, QPixmap
 from PySide6.QtWidgets import QGraphicsItem, QGraphicsEllipseItem, QGraphicsRectItem, QMenu, QGraphicsSceneMouseEvent
 
 from GridCalEngine.Devices.Branches.transformer3w import Transformer3W
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED
-from GridCal.Gui.BusBranchEditorWidget.terminal_item import TerminalItem
-from GridCal.Gui.BusBranchEditorWidget.Branches.winding_graphics import WindingGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Branches.winding_graphics import WindingGraphicItem
 from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class Transformer3WGraphicItem(QGraphicsRectItem):
     """
       Represents a block in the diagram
       Has an x and y and width and height
       width and height can only be adjusted with a tip in the lower right corner.
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/transformer_editor.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/transformer_editor.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Branches/line_graphics_template.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Branches/line_graphics_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,35 +18,35 @@
 import sys
 import numpy as np
 from typing import Union, TYPE_CHECKING
 from PySide6.QtCore import Qt, QLineF, QPointF, QRectF
 from PySide6.QtGui import QPen, QCursor, QPixmap, QBrush, QColor, QTransform, QPolygonF
 from PySide6.QtWidgets import (QGraphicsLineItem, QGraphicsRectItem, QGraphicsPolygonItem,
                                QGraphicsEllipseItem, QGraphicsSceneMouseEvent, QGraphicsTextItem)
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import TerminalItem
-from GridCal.Gui.BusBranchEditorWidget.Substation.bus_graphics import BusGraphicItem
-from GridCal.Gui.BusBranchEditorWidget.Fluid.fluid_node_graphics import FluidNodeGraphicItem
-
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, GenericDBWidget
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Substation.bus_graphics import BusGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Fluid.fluid_node_graphics import FluidNodeGraphicItem
 from GridCal.Gui.messages import yes_no_question
+
 from GridCalEngine.Devices.Substation.bus import Bus
 from GridCalEngine.Devices.Branches.line import Line
 from GridCalEngine.Devices.Branches.transformer import Transformer2W
 from GridCalEngine.Devices.Branches.winding import Winding
 from GridCalEngine.Devices.Branches.vsc import VSC
 from GridCalEngine.Devices.Branches.upfc import UPFC
 from GridCalEngine.Devices.Branches.dc_line import DcLine
 from GridCalEngine.Devices.Branches.series_reactance import SeriesReactance
 from GridCalEngine.Devices.Branches.hvdc_line import HvdcLine
 from GridCalEngine.Devices.Fluid.fluid_node import FluidNode
 from GridCalEngine.Devices.Fluid.fluid_path import FluidPath
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
-    from GridCal.Gui.BusBranchEditorWidget.Branches.transformer3w_graphics import Transformer3WGraphicItem
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget import Transformer3WGraphicItem
 
 
 class ArrowHead(QGraphicsPolygonItem):
     """
     This is the arrow object
     """
 
@@ -394,15 +394,15 @@
 
         transform = QTransform()
         transform.translate(center.x(), center.y())
         transform.rotate(np.rad2deg(ang))
         self.setTransform(transform)
 
 
-class LineGraphicTemplateItem(QGraphicsLineItem):
+class LineGraphicTemplateItem(GenericDBWidget, QGraphicsLineItem):
     """
     LineGraphicItem
     """
 
     def __init__(self,
                  from_port: TerminalItem,
                  to_port: Union[TerminalItem, None],
@@ -415,18 +415,17 @@
         :param from_port:
         :param to_port:
         :param editor:
         :param width:
         :param api_object:
         :param arrow_size:
         """
+        GenericDBWidget.__init__(self, parent=None, api_object=api_object, editor=editor, draw_labels=True)
         QGraphicsLineItem.__init__(self)
 
-        self.api_object = api_object
-
         if isinstance(api_object, Transformer2W):
             if isinstance(api_object, Winding):  # Winding is a sublass of Transformer
                 self.symbol = None
             else:
                 self.symbol = TransformerSymbol(parent=self, pen_width=width, h=80, w=80)
         elif isinstance(api_object, VSC):
             self.symbol = VscSymbol(parent=self, pen_width=width, h=48, w=48)
@@ -441,30 +440,17 @@
 
         self.scale = 1.0
         self.pen_style = Qt.SolidLine
         self.pen_color = Qt.black
         self.pen_width = width
         self.width = width
 
-        if self.api_object is not None:
-            if self.api_object.active:
-                self.color = ACTIVE['color']
-                self.style = ACTIVE['style']
-            else:
-                self.color = DEACTIVATED['color']
-                self.style = DEACTIVATED['style']
-        else:
-            self.color = ACTIVE['color']
-            self.style = ACTIVE['style']
-
         self.setFlag(self.GraphicsItemFlag.ItemIsSelectable, True)
         self.setCursor(QCursor(Qt.PointingHandCursor))
 
-        self.editor: BusBranchEditorWidget = editor
-
         self.pos1: QPointF = QPointF(0.0, 0.0)
         self.pos2: QPointF = QPointF(0.0, 0.0)
 
         self._from_port: Union[TerminalItem, None] = None
         self._to_port: Union[TerminalItem, None] = None
 
         # arrows
@@ -521,24 +507,15 @@
         self._from_port.update()
         self._to_port.update()
 
     def recolour_mode(self) -> None:
         """
         Change the colour according to the system theme
         """
-        if self.api_object is not None:
-            if self.api_object.active:
-                self.color = ACTIVE['color']
-                self.style = ACTIVE['style']
-            else:
-                self.color = DEACTIVATED['color']
-                self.style = DEACTIVATED['style']
-        else:
-            self.color = ACTIVE['color']
-            self.style = ACTIVE['style']
+        super().recolour_mode()
 
         self.set_colour(self.color, self.width, self.style)
 
     def set_colour(self, color: QColor, w, style: Qt.PenStyle):
         """
         Set color and style
         :param color: QColor instance
@@ -859,27 +836,27 @@
     def is_from_port_a_tr3(self) -> bool:
         """
 
         :return:
         """
         if self._from_port:
             if 'Transformer3WGraphicItem' not in sys.modules:
-                from GridCal.Gui.BusBranchEditorWidget.Branches.transformer3w_graphics import Transformer3WGraphicItem
+                from GridCal.Gui.Diagrams.BusBranchEditorWidget import Transformer3WGraphicItem
             return isinstance(self.get_terminal_from_parent(), Transformer3WGraphicItem)
         else:
             return False
 
     def is_to_port_a_tr3(self) -> bool:
         """
 
         :return:
         """
         if self._to_port:
             if 'Transformer3WGraphicItem' not in sys.modules:
-                from GridCal.Gui.BusBranchEditorWidget.Branches.transformer3w_graphics import Transformer3WGraphicItem
+                from GridCal.Gui.Diagrams.BusBranchEditorWidget import Transformer3WGraphicItem
             return isinstance(self.get_terminal_to_parent(), Transformer3WGraphicItem)
         else:
             return False
 
     def is_from_port_a_fluid_node(self) -> bool:
         """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/static_generator_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/static_generator_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,20 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import Union, TYPE_CHECKING
 from PySide6.QtGui import QPen, QIcon, QPixmap
 from PySide6.QtWidgets import QMenu, QGraphicsTextItem
 from GridCalEngine.Devices.Injections.static_generator import StaticGenerator, DeviceType
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
-from GridCal.Gui.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
-from GridCal.Gui.GuiFunctions import ObjectsModel
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class StaticGeneratorGraphicItem(InjectionTemplateGraphicItem):
 
     def __init__(self, parent, api_obj: StaticGenerator, editor: "BusBranchEditorWidget"):
         """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/current_injection_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/current_injection_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6 import QtWidgets, QtGui, QtCore
 from GridCalEngine.Devices.Injections.current_injection import CurrentInjection, DeviceType
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
-from GridCal.Gui.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class CurrentInjectionGraphicItem(InjectionTemplateGraphicItem):
     """
     ExternalGrid graphic item
     """
     def __init__(self, parent, api_obj: CurrentInjection, editor: BusBranchEditorWidget):
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/injections_template_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/injections_template_graphics.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,89 +15,72 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtCore import Qt
 from PySide6.QtGui import QPen, QCursor
 from PySide6.QtWidgets import QGraphicsLineItem, QGraphicsItemGroup
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER
 from GridCal.Gui.messages import yes_no_question, error_msg, warning_msg
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import GenericDBWidget
 from GridCalEngine.enumerations import DeviceType
 from GridCalEngine.Devices.types import INJECTION_DEVICE_TYPES
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
-class InjectionTemplateGraphicItem(QGraphicsItemGroup):
+class InjectionTemplateGraphicItem(GenericDBWidget, QGraphicsItemGroup):
     """
     InjectionTemplateGraphicItem
     """
 
     def __init__(self,
                  parent,
                  api_obj: INJECTION_DEVICE_TYPES,
                  device_type_name: str,
                  w: int,
                  h: int,
-                 editor: "BusBranchEditorWidget"):
+                 editor: BusBranchEditorWidget):
         """
 
         :param parent:
         :param api_obj:
         :param device_type_name:
         :param w:
         :param h:
         """
-        super(InjectionTemplateGraphicItem, self).__init__(parent)
+        GenericDBWidget.__init__(self, parent=parent, api_object=api_obj, editor=editor, draw_labels=True)
+        QGraphicsItemGroup.__init__(self, parent)
 
         self.w = w
         self.h = h
 
         self.scale = 1.0
 
-        self.parent = parent
-
-        self.api_object = api_obj
-
-        self.editor = editor
-
         self.device_type_name = device_type_name
 
         # Properties of the container:
         self.setFlags(self.GraphicsItemFlag.ItemIsSelectable | self.GraphicsItemFlag.ItemIsMovable)
         self.setCursor(QCursor(Qt.PointingHandCursor))
 
         self.width = 4
 
-        self.style = OTHER['style']
-        self.color = OTHER['color']
-
         # line to tie this object with the original bus (the parent)
         self.nexus = QGraphicsLineItem()
         self.nexus.setPen(QPen(self.color, self.width, self.style))
         self.editor.add_to_scene(self.nexus)
 
         self.setPos(self.parent.x(), self.parent.y() + 100)
         self.update_nexus(self.pos())
 
     def recolour_mode(self):
         """
         Change the colour according to the system theme
         """
-        if self.api_object is not None:
-            if self.api_object.active:
-                self.color = ACTIVE['color']
-                self.style = ACTIVE['style']
-            else:
-                self.color = DEACTIVATED['color']
-                self.style = DEACTIVATED['style']
-        else:
-            self.color = ACTIVE['color']
-            self.style = ACTIVE['style']
+        super().recolour_mode()
 
         pen = QPen(self.color, self.width, self.style)
         self.nexus.setPen(pen)
         return pen
 
     def update_nexus(self, pos):
         """
@@ -118,16 +101,16 @@
 
     def remove(self, ask=True):
         """
         Remove this element
         @return:
         """
         if ask:
-            ok = yes_no_question('Are you sure that you want to remove this ' + self.device_type_name + '?',
-                                 'Remove ' + self.api_object.name)
+            ok = yes_no_question(f'Are you sure that you want to remove this {self.device_type_name}?',
+                                 f'Remove {self.api_object.name}')
         else:
             ok = True
 
         if ok:
             self.editor.remove_from_scene(self.nexus)
             self.editor.remove_element(device=self.api_object, graphic_object=self)
             self.editor.remove_from_scene(self)
@@ -159,22 +142,26 @@
                 idx, new_bus, new_bus_graphic_item = idx_bus_list[0]
                 idx, old_bus, old_bus_graphic_item = idx_bus_list[1]
             else:
                 error_msg("The bus to change has not been selected!", 'Change bus')
                 return
 
             ok = yes_no_question(
-                text="Are you sure that you want to relocate the bus from {0} to {1}?".format(old_bus.name,
-                                                                                              new_bus.name),
+                text=f"Are you sure that you want to relocate the bus from {old_bus.name} to {new_bus.name}?",
                 title='Change bus')
 
             if ok:
                 self.api_object.bus = new_bus
                 new_bus_graphic_item.add_object(api_obj=self.api_object)
                 new_bus_graphic_item.update()
                 self.remove(ask=False)
         else:
             warning_msg("you have to select the origin and destination buses!",
                         title='Change bus')
 
     def rescale(self, scale: float = 1.0):
-        self.scale = scale
+        """
+
+        :param scale:
+        :return:
+        """
+        self.scale = scale
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/battery_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/battery_graphics.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6 import QtWidgets, QtGui
 from GridCalEngine.Devices.Injections.battery import Battery, DeviceType
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
-from GridCal.Gui.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.GuiFunctions import ObjectsModel
 from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class BatteryGraphicItem(InjectionTemplateGraphicItem):
 
     def __init__(self, parent, api_obj: Battery, editor: BusBranchEditorWidget):
         """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/shunt_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/shunt_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6 import QtWidgets
 from PySide6.QtCore import QPointF, QLineF
 from PySide6.QtGui import QPen, QIcon, QPixmap
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Line
-from GridCal.Gui.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Line
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.messages import yes_no_question
 from GridCalEngine.Devices.Injections.shunt import Shunt
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class ShuntGraphicItem(InjectionTemplateGraphicItem):
 
     def __init__(self, parent, api_obj: Shunt, editor: "BusBranchEditorWidget"):
         """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/external_grid_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/external_grid_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6 import QtWidgets, QtGui, QtCore
 from GridCalEngine.Devices.Injections.external_grid import ExternalGrid, DeviceType
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
-from GridCal.Gui.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.GuiFunctions import ObjectsModel
 from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget import BusBranchEditorWidget
 
 
 class ExternalGridGraphicItem(InjectionTemplateGraphicItem):
     """
     ExternalGrid graphic item
     """
     def __init__(self, parent, api_obj: ExternalGrid, editor: BusBranchEditorWidget):
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/controllable_shunt_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/controllable_shunt_graphics.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 # You should have received a copy of the GNU Lesser General Public License
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6 import QtWidgets, QtGui
 from GridCalEngine.Devices.Injections.controllable_shunt import ControllableShunt, DeviceType
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
-from GridCal.Gui.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Square
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.messages import yes_no_question
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class ControllableShuntGraphicItem(InjectionTemplateGraphicItem):
     """
     ExternalGrid graphic item
     """
     def __init__(self, parent, api_obj: ControllableShunt, editor: BusBranchEditorWidget):
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/load_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/load_graphics.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,22 +15,21 @@
 # along with this program; if not, write to the Free Software Foundation,
 # Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301, USA.
 from __future__ import annotations
 from typing import TYPE_CHECKING
 from PySide6.QtCore import QPointF
 from PySide6.QtGui import QPen, QIcon, QPixmap, QPolygonF
 from PySide6.QtWidgets import QMenu
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER
-from GridCal.Gui.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Polygon
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.messages import yes_no_question
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import Polygon
 from GridCalEngine.Devices.Injections.load import Load
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class LoadGraphicItem(InjectionTemplateGraphicItem):
 
     def __init__(self, parent, api_obj: Load, editor: BusBranchEditorWidget):
         """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Injections/generator_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Injections/generator_graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 from PySide6.QtCore import Qt, QAbstractTableModel, QModelIndex, QPointF
 from PySide6.QtGui import QPen, QIcon, QPixmap, QFont
 from PySide6.QtWidgets import (QMenu, QGraphicsTextItem, QDialog, QTableView, QVBoxLayout, QHBoxLayout,
                                QPushButton, QSplitter, QFrame, QSpacerItem, QSizePolicy)
 from GridCalEngine.Devices.Injections.generator import Generator
 from GridCalEngine.Devices.Injections.generator_q_curve import GeneratorQCurve
 from GridCalEngine.basic_structures import Mat, Vec
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
-from GridCal.Gui.BusBranchEditorWidget.matplotlibwidget import MatplotlibWidget
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, OTHER, Circle
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.matplotlibwidget import MatplotlibWidget
 from GridCal.Gui.messages import yes_no_question, info_msg
-from GridCal.Gui.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.injections_template_graphics import InjectionTemplateGraphicItem
 from GridCal.Gui.SolarPowerWizard.solar_power_wizzard import SolarPvWizard
 from GridCal.Gui.WindPowerWizard.wind_power_wizzard import WindFarmWizard
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
 class GeneratorQCurveEditorTableModel(QAbstractTableModel):
     """
     GeneratorQCurveEditorTableModel
     """
```

### Comparing `GridCal-5.1.0/GridCal/Gui/BusBranchEditorWidget/Substation/bus_graphics.py` & `GridCal-5.1.1/GridCal/Gui/Diagrams/BusBranchEditorWidget/Substation/cn_graphics.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,39 +17,44 @@
 from __future__ import annotations
 import numpy as np
 from typing import Union, TYPE_CHECKING, List, Dict
 from PySide6 import QtWidgets
 from PySide6.QtCore import Qt, QPoint, QRectF, QRect
 from PySide6.QtGui import QPen, QCursor, QIcon, QPixmap, QBrush, QColor
 from PySide6.QtWidgets import QMenu, QGraphicsSceneMouseEvent
-from GridCalEngine.Devices.Substation import Bus
-from GridCal.Gui.BusBranchEditorWidget.generic_graphics import ACTIVE, DEACTIVATED, FONT_SCALE, EMERGENCY
-from GridCalEngine.Simulations.Topology.topology_reduction_driver import reduce_buses
-from GridCal.Gui.BusBranchEditorWidget.terminal_item import TerminalItem, HandleItem
-from GridCal.Gui.BusBranchEditorWidget.Injections.load_graphics import LoadGraphicItem, Load
-from GridCal.Gui.BusBranchEditorWidget.Injections.generator_graphics import GeneratorGraphicItem, Generator
-from GridCal.Gui.BusBranchEditorWidget.Injections.static_generator_graphics import (StaticGeneratorGraphicItem,
-                                                                                    StaticGenerator)
-from GridCal.Gui.BusBranchEditorWidget.Injections.battery_graphics import (BatteryGraphicItem, Battery)
-from GridCal.Gui.BusBranchEditorWidget.Injections.shunt_graphics import (ShuntGraphicItem, Shunt)
-from GridCal.Gui.BusBranchEditorWidget.Injections.external_grid_graphics import (ExternalGridGraphicItem, ExternalGrid)
-from GridCal.Gui.BusBranchEditorWidget.Injections.current_injection_graphics import (CurrentInjectionGraphicItem,
-                                                                                     CurrentInjection)
-from GridCal.Gui.BusBranchEditorWidget.Injections.controllable_shunt_graphics import (ControllableShuntGraphicItem,
-                                                                                      ControllableShunt)
+
 from GridCal.Gui.messages import yes_no_question
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.generic_graphics import (GenericDBWidget, ACTIVE, DEACTIVATED,
+                                                                         FONT_SCALE, EMERGENCY)
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.terminal_item import TerminalItem, HandleItem
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.load_graphics import LoadGraphicItem, Load
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.generator_graphics import GeneratorGraphicItem, Generator
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.static_generator_graphics import (StaticGeneratorGraphicItem,
+                                                                                             StaticGenerator)
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.battery_graphics import (BatteryGraphicItem, Battery)
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.shunt_graphics import (ShuntGraphicItem, Shunt)
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.external_grid_graphics import (ExternalGridGraphicItem,
+                                                                                          ExternalGrid)
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.current_injection_graphics import (
+    CurrentInjectionGraphicItem,
+    CurrentInjection)
+from GridCal.Gui.Diagrams.BusBranchEditorWidget.Injections.controllable_shunt_graphics import (
+    ControllableShuntGraphicItem,
+    ControllableShunt)
+
 from GridCalEngine.enumerations import DeviceType, FaultType
-# from GridCalEngine.Devices.Parents.editable_device import EditableDevice
 from GridCalEngine.Devices.types import INJECTION_DEVICE_TYPES
+from GridCalEngine.Simulations.Topology.topology_reduction_driver import reduce_buses
+from GridCalEngine.Devices.Substation import Bus
 
 if TYPE_CHECKING:  # Only imports the below statements during type checking
-    from GridCal.Gui.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
+    from GridCal.Gui.Diagrams.BusBranchEditorWidget.bus_branch_editor_widget import BusBranchEditorWidget
 
 
-class BusGraphicItem(QtWidgets.QGraphicsRectItem):
+class CnGraphicItem(GenericDBWidget, QtWidgets.QGraphicsRectItem):
     """
       Represents a block in the diagram
       Has an x and y and width and height
       width and height can only be adjusted with a tip in the lower right corner.
 
       - in and output ports
       - parameters
@@ -72,49 +77,34 @@
         :param editor:
         :param bus:
         :param h:
         :param w:
         :param x:
         :param y:
         """
-        super(BusGraphicItem, self).__init__(parent)
+        GenericDBWidget.__init__(self, parent=parent, api_object=bus, editor=editor, draw_labels=True)
+        QtWidgets.QGraphicsRectItem.__init__(self, parent)
 
         self.min_w = 180.0
         self.min_h = 40.0
         self.offset = 20
         self.h = h if h >= self.min_h else self.min_h
         self.w = w if w >= self.min_w else self.min_w
 
-        self.api_object = bus
-
-        self.editor = editor
-
         # loads, shunts, generators, etc...
         self.shunt_children = list()
 
         # Enabled for short circuit
         self.sc_enabled = [False, False, False, False]
         self.sc_type = FaultType.ph3
         self.pen_width = 4
 
         # index
         self.index = index
 
-        # color
-        if self.api_object is not None:
-            if self.api_object.active:
-                self.color = ACTIVE['color']
-                self.style = ACTIVE['style']
-            else:
-                self.color = DEACTIVATED['color']
-                self.style = DEACTIVATED['style']
-        else:
-            self.color = ACTIVE['color']
-            self.style = ACTIVE['style']
-
         # Label:
         self.label = QtWidgets.QGraphicsTextItem(self.api_object.name if self.api_object is not None else "", self)
         self.label.setDefaultTextColor(ACTIVE['text'])
         self.label.setScale(FONT_SCALE)
 
         # square
         self.tile = QtWidgets.QGraphicsRectItem(0, 0, 20, 20, self)
@@ -143,24 +133,15 @@
 
         self.set_position(x, y)
 
     def recolour_mode(self) -> None:
         """
         Change the colour according to the system theme
         """
-        if self.api_object is not None:
-            if self.api_object.active:
-                self.color = ACTIVE['color']
-                self.style = ACTIVE['style']
-            else:
-                self.color = DEACTIVATED['color']
-                self.style = DEACTIVATED['style']
-        else:
-            self.color = ACTIVE['color']
-            self.style = ACTIVE['style']
+        super().recolour_mode()
 
         self.label.setDefaultTextColor(ACTIVE['text'])
         self.set_tile_color(self.color)
 
         for e in self.shunt_children:
             if e is not None:
                 e.recolour_mode()
```

### Comparing `GridCal-5.1.0/GridCal/Gui/SigmaAnalysis/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/SigmaAnalysis/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/SigmaAnalysis/gui.py` & `GridCal-5.1.1/GridCal/Gui/SigmaAnalysis/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py` & `GridCal-5.1.1/GridCal/Gui/SigmaAnalysis/sigma_analysis_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/GridGenerator/grid_generator_dialogue.py` & `GridCal-5.1.1/GridCal/Gui/GridGenerator/grid_generator_dialogue.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/GridGenerator/icons_rc.py` & `GridCal-5.1.1/GridCal/Gui/GridGenerator/icons_rc.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/GridCal/Gui/GridGenerator/gui.py` & `GridCal-5.1.1/GridCal/Gui/GridGenerator/gui.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/setup.py` & `GridCal-5.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `GridCal-5.1.0/PKG-INFO` & `GridCal-5.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GridCal
-Version: 5.1.0
+Version: 5.1.1
 Summary: GridCal is a Power Systems simulation program intended for professional use and research
 Home-page: https://github.com/SanPen/GridCal
 Author: Santiago Peñate Vera et. Al.
 Author-email: santiago@gridcal.org
 License: LGPL
 Keywords: power systems planning
 Classifier:  License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
```


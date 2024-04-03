# Comparing `tmp/SimulationSimpleDatabase-22.6.2.tar.gz` & `tmp/SimulationSimpleDatabase-24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimulationSimpleDatabase-22.6.2.tar", last modified: Mon Nov 14 14:38:22 2022, max compression
+gzip compressed data, was "SimulationSimpleDatabase-24.1.tar", last modified: Wed Apr  3 13:05:14 2024, max compression
```

## Comparing `SimulationSimpleDatabase-22.6.2.tar` & `SimulationSimpleDatabase-24.1.tar`

### file list

```diff
@@ -1,40 +1,89 @@
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2022-11-14 14:38:22.098193 SimulationSimpleDatabase-22.6.2/
--rw-rw-r--   0 robin     (1000) robin     (1000)      243 2022-11-14 14:38:22.098193 SimulationSimpleDatabase-22.6.2/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)     3045 2022-10-05 07:40:24.000000 SimulationSimpleDatabase-22.6.2/README.md
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2022-11-14 14:38:22.094193 SimulationSimpleDatabase-22.6.2/SimulationSimpleDatabase.egg-info/
--rw-rw-r--   0 robin     (1000) robin     (1000)      243 2022-11-14 14:38:22.000000 SimulationSimpleDatabase-22.6.2/SimulationSimpleDatabase.egg-info/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)      938 2022-11-14 14:38:22.000000 SimulationSimpleDatabase-22.6.2/SimulationSimpleDatabase.egg-info/SOURCES.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        1 2022-11-14 14:38:22.000000 SimulationSimpleDatabase-22.6.2/SimulationSimpleDatabase.egg-info/dependency_links.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       18 2022-11-14 14:38:22.000000 SimulationSimpleDatabase-22.6.2/SimulationSimpleDatabase.egg-info/requires.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        4 2022-11-14 14:38:22.000000 SimulationSimpleDatabase-22.6.2/SimulationSimpleDatabase.egg-info/top_level.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       38 2022-11-14 14:38:22.098193 SimulationSimpleDatabase-22.6.2/setup.cfg
--rw-rw-r--   0 robin     (1000) robin     (1000)      986 2022-11-14 14:33:42.000000 SimulationSimpleDatabase-22.6.2/setup.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2022-11-14 14:38:22.094193 SimulationSimpleDatabase-22.6.2/src/
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2022-11-14 14:38:22.094193 SimulationSimpleDatabase-22.6.2/src/Core/
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2022-11-14 14:38:22.094193 SimulationSimpleDatabase-22.6.2/src/Core/Rendering/
--rw-rw-r--   0 robin     (1000) robin     (1000)     5603 2022-11-10 15:40:31.000000 SimulationSimpleDatabase-22.6.2/src/Core/Rendering/ReplayVisualizer.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     8985 2022-11-10 14:59:16.000000 SimulationSimpleDatabase-22.6.2/src/Core/Rendering/VedoActor.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    15472 2022-11-07 10:07:33.000000 SimulationSimpleDatabase-22.6.2/src/Core/Rendering/VedoFactory.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     9070 2022-11-10 14:51:16.000000 SimulationSimpleDatabase-22.6.2/src/Core/Rendering/VedoTable.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     9041 2022-11-07 10:28:31.000000 SimulationSimpleDatabase-22.6.2/src/Core/Rendering/VedoVisualizer.py
--rw-rw-r--   0 robin     (1000) robin     (1000)        0 2022-09-13 15:48:12.000000 SimulationSimpleDatabase-22.6.2/src/Core/Rendering/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2022-11-14 14:38:22.098193 SimulationSimpleDatabase-22.6.2/src/Core/Storage/
--rw-rw-r--   0 robin     (1000) robin     (1000)     6051 2022-10-20 14:03:17.000000 SimulationSimpleDatabase-22.6.2/src/Core/Storage/AdaptiveTable.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    30861 2022-11-02 10:42:17.000000 SimulationSimpleDatabase-22.6.2/src/Core/Storage/Database.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1202 2022-09-28 14:20:00.000000 SimulationSimpleDatabase-22.6.2/src/Core/Storage/Exporter.py
--rw-rw-r--   0 robin     (1000) robin     (1000)      365 2022-09-28 14:20:00.000000 SimulationSimpleDatabase-22.6.2/src/Core/Storage/ExtendedFields.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     5739 2022-09-28 07:37:06.000000 SimulationSimpleDatabase-22.6.2/src/Core/Storage/ExtendedPeewee.py
--rw-rw-r--   0 robin     (1000) robin     (1000)        0 2022-09-16 15:59:01.000000 SimulationSimpleDatabase-22.6.2/src/Core/Storage/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     6786 2022-09-28 14:56:47.000000 SimulationSimpleDatabase-22.6.2/src/Core/Storage/utils.py
--rw-rw-r--   0 robin     (1000) robin     (1000)        0 2022-09-16 15:57:07.000000 SimulationSimpleDatabase-22.6.2/src/Core/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2022-11-14 14:38:22.098193 SimulationSimpleDatabase-22.6.2/src/SOFA/
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2022-11-14 14:38:22.098193 SimulationSimpleDatabase-22.6.2/src/SOFA/Rendering/
--rw-rw-r--   0 robin     (1000) robin     (1000)      587 2022-09-28 16:07:40.000000 SimulationSimpleDatabase-22.6.2/src/SOFA/Rendering/ReplayVisualizer.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    21641 2022-11-10 15:05:06.000000 SimulationSimpleDatabase-22.6.2/src/SOFA/Rendering/VedoFactory.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1083 2022-09-28 16:05:06.000000 SimulationSimpleDatabase-22.6.2/src/SOFA/Rendering/VedoVisualizer.py
--rw-rw-r--   0 robin     (1000) robin     (1000)        0 2022-09-15 16:05:24.000000 SimulationSimpleDatabase-22.6.2/src/SOFA/Rendering/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2022-11-14 14:38:22.098193 SimulationSimpleDatabase-22.6.2/src/SOFA/Storage/
--rw-rw-r--   0 robin     (1000) robin     (1000)     6667 2022-10-04 08:49:27.000000 SimulationSimpleDatabase-22.6.2/src/SOFA/Storage/Database.py
--rw-rw-r--   0 robin     (1000) robin     (1000)        0 2022-09-15 16:05:17.000000 SimulationSimpleDatabase-22.6.2/src/SOFA/Storage/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)        0 2022-09-15 16:04:35.000000 SimulationSimpleDatabase-22.6.2/src/SOFA/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1180 2022-10-03 09:30:33.000000 SimulationSimpleDatabase-22.6.2/src/SOFA/utils.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.656083 SimulationSimpleDatabase-24.1/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1068 2023-07-24 08:21:50.000000 SimulationSimpleDatabase-24.1/LICENSE
+-rw-r--r--   0 robin     (1000) robin     (1000)     3641 2024-04-03 13:05:14.656083 SimulationSimpleDatabase-24.1/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3145 2024-02-16 09:30:55.000000 SimulationSimpleDatabase-24.1/README.md
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.656083 SimulationSimpleDatabase-24.1/SimulationSimpleDatabase.egg-info/
+-rw-r--r--   0 robin     (1000) robin     (1000)     3641 2024-04-03 13:05:14.000000 SimulationSimpleDatabase-24.1/SimulationSimpleDatabase.egg-info/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2425 2024-04-03 13:05:14.000000 SimulationSimpleDatabase-24.1/SimulationSimpleDatabase.egg-info/SOURCES.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)        1 2024-04-03 13:05:14.000000 SimulationSimpleDatabase-24.1/SimulationSimpleDatabase.egg-info/dependency_links.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       44 2024-04-03 13:05:14.000000 SimulationSimpleDatabase-24.1/SimulationSimpleDatabase.egg-info/entry_points.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       77 2024-04-03 13:05:14.000000 SimulationSimpleDatabase-24.1/SimulationSimpleDatabase.egg-info/requires.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)        4 2024-04-03 13:05:14.000000 SimulationSimpleDatabase-24.1/SimulationSimpleDatabase.egg-info/top_level.txt
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.648083 SimulationSimpleDatabase-24.1/examples/
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.648083 SimulationSimpleDatabase-24.1/examples/Core/
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.648083 SimulationSimpleDatabase-24.1/examples/Core/rendering/
+-rw-rw-r--   0 robin     (1000) robin     (1000)   969837 2023-07-24 08:21:50.000000 SimulationSimpleDatabase-24.1/examples/Core/rendering/armadillo.obj
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1647 2024-02-01 10:30:37.000000 SimulationSimpleDatabase-24.1/examples/Core/rendering/offscreen.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      378 2024-02-01 10:30:37.000000 SimulationSimpleDatabase-24.1/examples/Core/rendering/replay.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2574 2024-02-01 10:31:28.000000 SimulationSimpleDatabase-24.1/examples/Core/rendering/several_factories.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2193 2024-02-01 10:31:56.000000 SimulationSimpleDatabase-24.1/examples/Core/rendering/several_factories_offscreen.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3321 2024-02-01 10:29:30.000000 SimulationSimpleDatabase-24.1/examples/Core/rendering/visualization.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.652083 SimulationSimpleDatabase-24.1/examples/Core/storage/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4765 2024-01-31 16:33:47.000000 SimulationSimpleDatabase-24.1/examples/Core/storage/foreignkey_db.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1336 2024-01-31 16:29:05.000000 SimulationSimpleDatabase-24.1/examples/Core/storage/read_db.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1414 2024-01-31 16:32:19.000000 SimulationSimpleDatabase-24.1/examples/Core/storage/signal_db.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1105 2024-01-31 16:31:15.000000 SimulationSimpleDatabase-24.1/examples/Core/storage/update_db.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1510 2024-04-03 09:08:08.000000 SimulationSimpleDatabase-24.1/examples/Core/storage/utils_db.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2012 2024-01-31 16:11:49.000000 SimulationSimpleDatabase-24.1/examples/Core/storage/write_db.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.648083 SimulationSimpleDatabase-24.1/examples/SOFA/
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.652083 SimulationSimpleDatabase-24.1/examples/SOFA/rendering/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5504 2024-02-07 15:41:11.000000 SimulationSimpleDatabase-24.1/examples/SOFA/rendering/Liver.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      876 2024-02-01 16:29:22.000000 SimulationSimpleDatabase-24.1/examples/SOFA/rendering/record.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      236 2024-02-07 15:46:18.000000 SimulationSimpleDatabase-24.1/examples/SOFA/rendering/replay.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.652083 SimulationSimpleDatabase-24.1/examples/SOFA/rendering-offscreen/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     9252 2024-02-07 15:50:21.000000 SimulationSimpleDatabase-24.1/examples/SOFA/rendering-offscreen/Caduceus.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      905 2024-02-07 15:50:21.000000 SimulationSimpleDatabase-24.1/examples/SOFA/rendering-offscreen/record.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      250 2024-02-07 15:50:21.000000 SimulationSimpleDatabase-24.1/examples/SOFA/rendering-offscreen/replay.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.652083 SimulationSimpleDatabase-24.1/examples/SOFA/storage/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     9737 2024-02-01 16:24:51.000000 SimulationSimpleDatabase-24.1/examples/SOFA/storage/Caduceus.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      670 2023-07-24 08:21:50.000000 SimulationSimpleDatabase-24.1/examples/SOFA/storage/record.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)       38 2024-04-03 13:05:14.656083 SimulationSimpleDatabase-24.1/setup.cfg
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1702 2024-04-03 11:54:16.000000 SimulationSimpleDatabase-24.1/setup.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.652083 SimulationSimpleDatabase-24.1/src/
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.652083 SimulationSimpleDatabase-24.1/src/Core/
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.652083 SimulationSimpleDatabase-24.1/src/Core/Rendering/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       92 2024-02-01 09:49:49.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.652083 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-07-24 08:21:50.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3379 2024-02-01 09:06:57.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/base_object.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5468 2024-02-01 09:18:11.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/base_replay.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     9436 2024-02-01 10:25:20.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/base_visualizer.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.652083 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/open3d/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-07-24 08:21:50.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/open3d/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    12747 2023-07-24 08:21:50.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/open3d/open3d_app.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    14650 2024-02-01 13:49:00.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/open3d/open3d_object.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6065 2024-02-01 13:49:00.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/open3d/open3d_replay.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     8226 2024-02-01 13:49:00.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/open3d/open3d_visualizer.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      817 2023-07-24 08:21:50.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/open3d/utils.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6051 2024-02-01 09:03:41.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/rendering_table.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.652083 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/vedo/
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-07-24 08:21:50.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/vedo/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      561 2024-02-01 13:43:17.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/vedo/utils.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     8772 2024-02-01 10:10:47.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/vedo/vedo_objet.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3693 2024-04-03 09:41:47.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/vedo/vedo_replay.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6550 2024-02-01 13:43:17.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/vedo/vedo_visualizer.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1595 2024-02-01 13:49:00.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/replay.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    18672 2024-02-01 09:49:49.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/user_api.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5225 2024-02-01 13:49:00.000000 SimulationSimpleDatabase-24.1/src/Core/Rendering/visualizer.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.656083 SimulationSimpleDatabase-24.1/src/Core/Storage/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      122 2024-01-31 16:14:37.000000 SimulationSimpleDatabase-24.1/src/Core/Storage/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6303 2024-01-31 16:17:46.000000 SimulationSimpleDatabase-24.1/src/Core/Storage/adaptive_table.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    31478 2024-01-31 17:24:46.000000 SimulationSimpleDatabase-24.1/src/Core/Storage/database.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1002 2024-01-31 14:30:45.000000 SimulationSimpleDatabase-24.1/src/Core/Storage/exporter.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      325 2024-01-31 16:16:28.000000 SimulationSimpleDatabase-24.1/src/Core/Storage/numpy_field.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5932 2024-01-31 16:16:28.000000 SimulationSimpleDatabase-24.1/src/Core/Storage/peewee_extension.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7130 2024-01-31 17:22:02.000000 SimulationSimpleDatabase-24.1/src/Core/Storage/utils.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2024-01-31 14:51:54.000000 SimulationSimpleDatabase-24.1/src/Core/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.656083 SimulationSimpleDatabase-24.1/src/SOFA/
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.656083 SimulationSimpleDatabase-24.1/src/SOFA/Rendering/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       92 2024-02-01 16:34:39.000000 SimulationSimpleDatabase-24.1/src/SOFA/Rendering/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      799 2024-02-01 16:34:39.000000 SimulationSimpleDatabase-24.1/src/SOFA/Rendering/replay.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    18727 2024-02-01 16:34:39.000000 SimulationSimpleDatabase-24.1/src/SOFA/Rendering/user_api.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1599 2024-02-01 16:34:39.000000 SimulationSimpleDatabase-24.1/src/SOFA/Rendering/visualizer.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2024-04-03 13:05:14.656083 SimulationSimpleDatabase-24.1/src/SOFA/Storage/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       31 2024-02-01 14:39:39.000000 SimulationSimpleDatabase-24.1/src/SOFA/Storage/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     6784 2024-02-01 14:39:39.000000 SimulationSimpleDatabase-24.1/src/SOFA/Storage/database.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2024-02-01 16:32:48.000000 SimulationSimpleDatabase-24.1/src/SOFA/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1180 2023-07-24 08:21:50.000000 SimulationSimpleDatabase-24.1/src/SOFA/utils.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)        0 2023-07-24 08:21:50.000000 SimulationSimpleDatabase-24.1/src/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     9410 2024-04-03 09:30:09.000000 SimulationSimpleDatabase-24.1/src/cli.py
```

### Comparing `SimulationSimpleDatabase-22.6.2/README.md` & `SimulationSimpleDatabase-24.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # SimulationSimpleDatabase (SSD)
 
 ![logo](docs/src/_static/images/logo.svg)
 
-The **SSD** project provides Python3 tools allowing users to easily develop **data storage** strategies for their
-**numerical simulations**.
+The **SSD** project provides Python3 tools allowing users to easily develop **data storage** and **visualization** 
+strategies for their **numerical simulations** with a minimal lines of code.
 
 This project has two main objectives:
 * Easy **storage** management system for **any data** from a numerical simulation;
 * Easy **storage** & **rendering** management systems for **visual data** from a numerical simulation.
 
 The **SSD** project is mainly using the [Peewee](http://docs.peewee-orm.com/en/latest/) Python3 library and was mostly 
-designed to fit the [DeepPhysX](https://github.com/mimesis-inria/DeepPhysX) and 
-[SOFA](https://www.sofa-framework.org/) frameworks.
+designed to fit the [**DeepPhysX**](https://github.com/mimesis-inria/DeepPhysX) and 
+[**SOFA**](https://www.sofa-framework.org/) frameworks.
 
 Discover more about the project on the dedicated 
 [**Documentation**](https://simulationsimpledatabase.readthedocs.io/en/latest/).
 
 ## Features
 
 The **SSD** project provides the following `Core` packages:
@@ -26,15 +26,15 @@
   * Event management system;
   * Tools such as merging and exporting data in other formats.
 * `SSD.Core.Rendering`
   * Automatic management of Database file for visualization data;
   * Live rendering of numerical simulations;
   * Replay of stored numerical simulation steps;
   * Various object types and highly customizable rendering styles;
-  * Several Python libraries available: [Vedo](https://vedo.embl.es/)
+  * Several Python libraries available: [Vedo](https://vedo.embl.es/), [Open3D](http://www.open3d.org/)
 
 The **SSD** project also provides a `SOFA` compatible package with additional features:
 * `SSD.SOFA.Storage`
   * Callbacks to automatically record any Data field of SOFA objects.
   * Recording can be done whether the simulation is running with *runSofa* or with a *python* interpreter.
 * `SSD.SOFA.Rendering`
   * Callbacks to automatically record visual Data fields of SOFA objects.
@@ -61,15 +61,15 @@
 $ git clone https://github.com/RobinEnjalbert/SimulationSimpleDatabase.git
 $ cd SimpleSimulationDatabase
 
 # Option 1: Install as non-editable (users)
 $ pip3 install .
 
 # Option 2: Install as editable (developers)
-$ python3 dev.py set
+$ python3 setup_dev.py set
 ```
 
 
 ## Gallery
 
 |      **examples/SOFA/rendering-offscreen/replay.py**      |
 |:---------------------------------------------------------:|
```

### Comparing `SimulationSimpleDatabase-22.6.2/src/Core/Rendering/ReplayVisualizer.py` & `SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/vedo/vedo_visualizer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,137 +1,189 @@
-from typing import Optional, Dict, Tuple
+import socket
+from typing import Dict, Optional
+from struct import unpack
 from vedo import show, Plotter
-from numpy import array, ndarray
+from threading import Thread
 
-from SSD.Core.Storage.Database import Database
-from SSD.Core.Rendering.VedoActor import VedoActor
+from SSD.Core.Storage.database import Database
+from SSD.Core.Rendering.backend.base_visualizer import BaseVisualizer
+from SSD.Core.Rendering.backend.vedo.vedo_objet import VedoObject
+from SSD.Core.Rendering.backend.vedo.utils import do_remove
 
 
-class ReplayVisualizer:
+class VedoVisualizer(BaseVisualizer):
 
     def __init__(self,
-                 database_name: str,
-                 database_dir: str = ''):
+                 database: Optional[Database] = None,
+                 database_dir: str = '',
+                 database_name: Optional[str] = None,
+                 remove_existing: bool = False,
+                 fps: int = 20):
+        """
+        The VedoVisualizer is used to manage the creation, update and rendering of Vedo Objects.
+
+        :param database: Database to connect to.
+        :param database_dir: Directory which contains the Database file (used if 'database' is not defined).
+        :param database_name: Name of the Database (used if 'database' is not defined).
+        :param remove_existing: If True, overwrite a Database with the same path.
+        :param fps: Max frame rate.
+        """
+
+        BaseVisualizer.__init__(self,
+                                database=database,
+                                database_dir=database_dir,
+                                database_name=database_name,
+                                remove_existing=remove_existing,
+                                fps=fps)
+
+        self.objects: Dict[int, Dict[str, VedoObject]] = {}
+        self.__plotter: Optional[Plotter] = None
+
+    def get_object(self,
+                   object_name: str) -> VedoObject:
         """
-        Replay a simulation from saved visual data.
+        Get an Object instance.
 
-        :param database_name: Name of the Database.
-        :param database_dir: Directory of the Database.
+        :param object_name: Name of the Object.
         """
 
-        # Load the Database
-        self.__database = Database(database_dir=database_dir, database_name=database_name).load()
+        group = self.groups[object_name]
+        return self.objects[group][object_name]
 
-        # Information about all Factories / Actors
-        self.__actors: Dict[int, Dict[Tuple[int, int], VedoActor]] = {}
-        self.__all_actors: Dict[Tuple[int, int], VedoActor] = {}
-        self.__updated_actors: Dict[Tuple[int, int], bool] = {}
-        self.__plotter: Optional[Plotter] = None
-        self.__nb_sample: Optional[int] = None
+    def create_object_backend(self,
+                              object_name: str,
+                              object_type: str,
+                              object_group: int) -> None:
+        """
+        Specific Object creation instructions.
+
+        :param object_name: Name of the Object.
+        :param object_type: Type of the Object.
+        :param object_group: Group of the Object.
+        """
 
-        # Init visualizer
-        self.step = 1
+        self.objects[object_group][object_name] = VedoObject(object_type=object_type,
+                                                             object_name=object_name,
+                                                             object_group=object_group)
 
-    def init_visualizer(self):
+    def launch_visualizer(self,
+                          nb_clients: int) -> None:
         """
-        Initialize the Visualizer: create all Actors and render them in a Plotter.
+        Start the Visualizer: create all Objects and render them.
+
+        :param nb_clients: Number of Factories to connect to.
         """
 
-        # 1. Get the Tables of the Database, sort their names per factory and per object indices
-        table_names = self.__database.get_tables()
-        table_names.remove('Sync')
-        sorted_table_names = []
-        sorter: Dict[int, Dict[int, str]] = {}
-        for table_name in table_names:
-            factory_id, table_id = table_name.split('_')[-2:]
-            if int(factory_id) not in sorter:
-                sorter[int(factory_id)] = {}
-            sorter[int(factory_id)][int(table_id)] = table_name
-        for factory_id in sorted(sorter.keys()):
-            for table_id in sorted(sorter[factory_id].keys()):
-                sorted_table_names.append(sorter[factory_id][table_id])
-
-        # 2. Retrieve visual data and create Actors (one Table per Actor)
-        instances = {}
-        for table_name in sorted_table_names:
-            # Get the number of sample
-            if self.__nb_sample is None:
-                self.__nb_sample = self.__database.nb_lines(table_name=table_name)
-            # Get the full line of data
-            data_dict = self.__database.get_line(table_name=table_name,
-                                                 line_id=1)
-            data_dict.pop('id')
-            # Sort data
-            cmap_dict = {'colormap': data_dict.pop('colormap') if 'colormap' in data_dict else 'jet',
-                         'scalar_field': data_dict.pop('scalar_field') if 'scalar_field' in data_dict else array([])}
-            at = data_dict.pop('at')
-            # Retrieve good indexing of Actors
-            actor_type, factory_id, actor_id = table_name.split('_')
-            factory_id, actor_id = int(factory_id), int(actor_id)
-            if at not in self.__actors:
-                self.__actors[at] = {}
-                instances[at] = []
-            # Create Actor
-            self.__actors[at][(factory_id, actor_id)] = VedoActor(self, actor_type, at)
-            self.__all_actors[(factory_id, actor_id)] = self.__actors[at][(factory_id, actor_id)]
-            self.__updated_actors[(factory_id, actor_id)] = False
-            instances[at].append(self.__actors[at][(factory_id, actor_id)].create(data_dict).apply_cmap(cmap_dict))
-
-        # 3. Create Plotter
-        actors = []
-        for window in sorted(instances.keys()):
-            actors.append(instances[window])
+        # 1. Create the list of objects to render
+        objects = []
+        for group in self.objects.keys():
+            objects.append([])
+            for v_object in self.objects[group].values():
+                objects[-1].append(v_object.instance)
 
-        self.__plotter = show(actors,
+        # 2. Create a non-interactive Plotter instance
+        self.__plotter = show(objects,
                               new=True,
-                              N=len(actors),
+                              N=len(objects),
                               sharecam=True,
                               interactive=False,
-                              title='SofaVedo',
+                              title='SSD',
                               axes=4)
-        self.__plotter.timer_callback('create')
-        self.__plotter.add_callback('Timer', self.__update)
-        self.__plotter.add_button(self.__start, states=['start'])
+
+        # 3. Add a timer callback and set the Plotter in interactive mode
+        timer_id = self.__plotter.timer_callback('create', dt=int(self.fps * 1e3) // nb_clients)
+        if nb_clients == 1:
+            self.__plotter.add_callback('timer', self.single_client_thread)
+            self.clients[0].send(b'done')
+        else:
+            self.__plotter.add_callback('timer', self.multiple_clients_thread)
+            for i, client in enumerate(self.clients):
+                client.send(b'done')
+                Thread(target=self.listen_client, args=(i,)).start()
         self.__plotter.interactive()
+        self.__plotter.timer_callback('destroy', timer_id=timer_id)
+        self.__plotter.close()
+        self.__plotter = None
 
-    def get_actor(self,
-                  actor_id: ndarray):
+        # 4. The window was closed
+        if False in self.is_done:
+            self.exit()
+
+    def single_client_thread(self, _) -> None:
+        """
+        Timer callback for a single Factory.
         """
-        Get an Actor instance.
 
-        :param actor_id: Index of the Actor.
+        try:
+            msg = self.clients[0].recv(4)
+            if len(msg) == 0:
+                pass
+            elif msg == b'exit':
+                self.is_done[0] = True
+                self.exit(force_quit=False)
+            else:
+                step = unpack('i', msg)[0]
+                self.update_visualizer(step=step, idx_factory=0)
+                self.clients[0].send(b'done')
+        except socket.timeout:
+            pass
+
+    def multiple_clients_thread(self, _) -> None:
         """
+        Timer callback for several Factories.
+        """
+
+        if len(self.requests) > 0:
+            i, step = self.requests.pop(0)
+            self.update_visualizer(step=step, idx_factory=i)
+            self.clients[i].send(b'done')
 
-        return self.__all_actors[tuple(actor_id)]
+    def update_visualizer(self,
+                          step: int,
+                          idx_factory: int) -> None:
+        """
+        Update the rendering view.
 
-    def __start(self):
+        :param step: Index of the current step.
+        :param idx_factory: Index of the Factory to update.
+        """
 
-        self.step = 1
+        self.update_objects(step=step,
+                            idx_factory=idx_factory)
+        self.__plotter.render()
 
-    def __update(self, _):
+    def update_object_backend(self,
+                              v_object: VedoObject) -> None:
+        """
+        Specific Object update instructions.
 
-        self.step += 1
-        if self.step < self.__nb_sample:
+        :param v_object: Object object.
+        """
+
+        removed = False
+        if do_remove(v_object, v_object.updated_fields):
+            self.__plotter.remove(v_object.instance, at=v_object.group)
+            removed = True
+        v_object.update()
+        if removed:
+            self.__plotter.add(v_object.instance, at=v_object.group)
+
+    def exit(self,
+             force_quit: bool = True) -> None:
+        """
+        Exit procedure of the Visualizer.
+
+        :param force_quit: True if the Window was manually closed.
+        """
 
-            # 1. Get the Tables of the Database
-            table_names = self.__database.get_tables()
-            table_names.remove('Sync')
+        if force_quit:
+            for i, client in enumerate(self.clients):
+                client.send(b'exit')
 
-            # 2. Retrieve visual data and create Actors (one Table per Actor)
-            for table_name in table_names:
-                # Get the full line of data
-                data_dict = self.__database.get_line(table_name=table_name, line_id=self.step)
-                data_dict.pop('id')
-                # Sort data
-                cmap_dict = {'scalar_field': data_dict.pop('scalar_field')} if 'scalar_field' in data_dict else {}
-                # Update Actors
-                _, factory_id, actor_id = table_name.split('_')
-                factory_id, actor_id = int(factory_id), int(actor_id)
-                actor = self.__all_actors[(factory_id, actor_id)]
-                if actor.actor_type in ['Arrows', 'Markers', 'Symbols']:
-                    self.__plotter.remove(actor.instance, at=actor.at)
-                actor.update(data_dict).apply_cmap(cmap_dict)
-                if actor.actor_type in ['Arrows', 'Markers', 'Symbols']:
-                    self.__plotter.add(actor.instance, at=actor.at)
+        # Close the socket
+        if self.server is not None:
+            self.server.close()
+            self.server = None
 
-            # 3. Render
-            self.__plotter.render()
+        # Close the Plotter
+        if self.__plotter is not None:
+            self.__plotter.break_interaction()
```

### Comparing `SimulationSimpleDatabase-22.6.2/src/Core/Rendering/VedoVisualizer.py` & `SimulationSimpleDatabase-24.1/src/Core/Rendering/backend/open3d/open3d_visualizer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,217 +1,225 @@
-from typing import Dict, Optional, Any, Tuple
-from numpy import array, ndarray
-from vedo import show, Plotter
+import socket
+from typing import Dict, Optional, Tuple
+from threading import Thread
+from struct import unpack
+from copy import copy
+from time import time, sleep
+import open3d.visualization.gui as gui
+
+from SSD.Core.Storage.database import Database
+from SSD.Core.Rendering.backend.base_visualizer import BaseVisualizer
+from SSD.Core.Rendering.backend.open3d.open3d_object import Open3dObject
+from SSD.Core.Rendering.backend.open3d.open3d_app import BaseApp
 
-from SSD.Core.Storage.Database import Database
-from SSD.Core.Rendering.VedoActor import VedoActor
 
-
-class VedoVisualizer:
+class Open3dVisualizer(BaseApp, BaseVisualizer):
 
     def __init__(self,
                  database: Optional[Database] = None,
                  database_dir: str = '',
                  database_name: Optional[str] = None,
                  remove_existing: bool = False,
-                 offscreen: bool = False):
+                 fps: int = 20):
         """
-        Manage the creation, update and rendering of Vedo Actors.
+        The Open3dVisualizer is used to manage the creation, update and rendering of Open3D Actors.
 
         :param database: Database to connect to.
         :param database_dir: Directory which contains the Database file (used if 'database' is not defined).
         :param database_name: Name of the Database (used if 'database' is not defined).
         :param remove_existing: If True, overwrite a Database with the same path.
-        :param offscreen: If True, visual data will be saved but not rendered.
+        :param fps: Max frame rate.
         """
 
-        # Define Database
-        if database is not None:
-            self.__database: Database = database
-        elif database_name is not None:
-            self.__database: Database = Database(database_dir=database_dir,
-                                                 database_name=database_name).new(remove_existing=remove_existing)
-        else:
-            raise ValueError("Both 'database' and 'database_name' are not defined.")
+        BaseVisualizer.__init__(self,
+                                database=database,
+                                database_dir=database_dir,
+                                database_name=database_name,
+                                remove_existing=remove_existing,
+                                fps=fps)
+
+        self.objects: Dict[int, Dict[str, Open3dObject]] = {}
+        self.__current_group: int = 0
+        self.__previous_group: int = 0
+        self.__group_change: bool = False
+        self.__step: Tuple[int, int] = (1, 1)
 
-        # Information about all Factories / Actors
-        self.__actors: Dict[int, Dict[Tuple[int, int], VedoActor]] = {}
-        self.__all_actors: Dict[Tuple[int, int], VedoActor] = {}
-        self.__plotter: Optional[Plotter] = None
-        self.__offscreen: bool = offscreen
-        self.step: int = 0
+    def get_object(self,
+                   object_name: str) -> Open3dObject:
+        """
+        Get an Actor instance.
 
-        self.__database.create_table(table_name='Sync',
-                                     storing_table=False,
-                                     fields=('step', str))
-        self.__database.register_post_save_signal(table_name='Sync',
-                                                  handler=self.__sync_visualizer)
+        :param object_name: Name of the Actor.
+        """
 
-    def get_database(self):
+        group = self.groups[object_name]
+        return self.objects[group][object_name]
+
+    def create_object_backend(self,
+                              object_name: str,
+                              object_type: str,
+                              object_group: int) -> None:
         """
-        Get the Database.
+        Specific Actor creation instructions.
+
+        :param object_name: Name of the Actor.
+        :param object_type: Type of the Actor.
+        :param object_group: Group of the Actor.
         """
 
-        return self.__database
+        self.objects[object_group][object_name] = Open3dObject(object_type=object_type,
+                                                               object_name=object_name,
+                                                               object_group=object_group)
+        if object_type == 'Text':
+            self.additional_labels[object_name] = self.objects[object_group][object_name]
 
-    def get_path(self):
+    def launch_visualizer(self,
+                          nb_clients: int) -> None:
         """
-        Get the path to the Database.
+        Start the Visualizer: create all Actors and render them.
+
+        :param nb_clients: Number of Factories to connect to.
         """
 
-        return self.__database.get_path()
+        # 1. Init Visualizer instance
+        self._create_settings(len(self.objects))
+        self._window.set_on_close(self.exit)
+
+        # 2 Add all Text
+        for v_object in self.additional_labels.values():
+            self._window.add_child(v_object.instance)
+            v_object.instance.visible = False
 
-    def get_actor(self,
-                  actor_id: ndarray):
+        # 3. Add geometries to the Visualizer
+        for v_object in self.objects[self.__current_group].values():
+            if v_object.type == 'Text':
+                v_object.instance.visible = True
+            else:
+                self._scene.scene.add_geometry(v_object.name, v_object.instance, v_object.material)
+        bounds = self._scene.scene.bounding_box
+        self._scene.setup_camera(60, bounds, bounds.get_center())
+
+        # 4. Launch mainloop
+        if nb_clients == 1:
+            Thread(target=self.single_client_thread).start()
+            self.clients[0].send(b'done')
+        else:
+            for i, client in enumerate(self.clients):
+                Thread(target=self.listen_client, args=(i,)).start()
+                client.send(b'done')
+            Thread(target=self.multiple_clients_thread).start()
+
+        gui.Application.instance.run()
+
+    def single_client_thread(self):
         """
-        Get an Actor instance.
+        Timer callback for a single Factory.
+        """
+
+        while not self.is_done[0]:
+            try:
+                msg = self.clients[0].recv(4)
+                if len(msg) == 0:
+                    pass
+                elif msg == b'exit':
+                    self.is_done[0] = True
+                    self.exit(force_quit=False)
+                else:
+                    self.__step = (0, unpack('i', msg)[0])
+                    process_time = time()
+                    gui.Application.instance.post_to_main_thread(self._window,
+                                                                 self.update_visualizer)
+                    dt = max(0., self.fps - (time() - process_time))
+                    sleep(dt)
+            except socket.timeout:
+                pass
+
+        gui.Application.instance.quit()
 
-        :param actor_id: Index of the Actor.
+    def multiple_clients_thread(self) -> None:
         """
+        Timer callback for several Factories.
+        """
+
+        while False in self.is_done:
+
+            if len(self.requests) > 0:
+                self.__step = self.requests.pop(0)
+                process_time = time()
+                gui.Application.instance.post_to_main_thread(self._window,
+                                                             self.update_visualizer)
+                dt = max(0., self.fps - (time() - process_time))
+                sleep(dt)
 
-        return self.__all_actors[tuple(actor_id)]
+        gui.Application.instance.quit()
 
-    def init_visualizer(self):
+    def update_visualizer(self) -> None:
         """
-        Initialize the Visualizer: create all Actors and render them in a Plotter.
+        Update the rendering view.
         """
 
-        # 1. Connect signals between the VedoFactory and the Visualizer
-        self.__database.connect_signals()
-
-        # 2. Sort the Table names per factory and per object indices
-        table_names = self.__database.get_tables()
-        table_names.remove('Sync')
-        sorted_table_names = []
-        sorter: Dict[int, Dict[int, str]] = {}
-        for table_name in table_names:
-            factory_id, table_id = table_name.split('_')[-2:]
-            if int(factory_id) not in sorter:
-                sorter[int(factory_id)] = {}
-            sorter[int(factory_id)][int(table_id)] = table_name
-        for factory_id in sorted(sorter.keys()):
-            for table_id in sorted(sorter[factory_id].keys()):
-                sorted_table_names.append(sorter[factory_id][table_id])
-
-        # 3.  Retrieve visual data and create Actors (one Table per Actor)
-        instances = {}
-        real_at = {}
-        for table_name in sorted_table_names:
-            # Get the full line of data
-            data_dict = self.__database.get_line(table_name=table_name)
-            data_dict.pop('id')
-            # Sort data
-            cmap_dict = {'colormap': data_dict.pop('colormap') if 'colormap' in data_dict else 'jet',
-                         'scalar_field': data_dict.pop('scalar_field') if 'scalar_field' in data_dict else array([])}
-            at = data_dict.pop('at')
-            # Retrieve good indexing of Actors
-            actor_type, factory_id, actor_id = table_name.split('_')
-            factory_id, actor_id = int(factory_id), int(actor_id)
-            if at not in self.__actors:
-                self.__actors[at] = {}
-                instances[at] = []
-                real_at[at] = []
-            # Create Actor
-            self.__actors[at][(factory_id, actor_id)] = VedoActor(self, actor_type, at)
-            self.__all_actors[(factory_id, actor_id)] = self.__actors[at][(factory_id, actor_id)]
-            instances[at].append(self.__actors[at][(factory_id, actor_id)].create(data_dict).apply_cmap(cmap_dict))
-            real_at[at].append(table_name)
-
-        # 4. Update the 'at' values
-        for i, at in enumerate(sorted(self.__actors.keys())):
-            # Update in the Database
-            if i != at:
-                for table_name in real_at[at]:
-                    self.__database.update(table_name=table_name,
-                                           data={'at': i})
-            # Update in Actors container
-            instances[i] = instances.pop(at)
-            # Update in Actors
-            for idx in self.__actors[at]:
-                self.__all_actors[idx].at = i
-
-        # 5. Create Plotter if offscreen is False
-        if not self.__offscreen:
-            actors = []
-            for window in sorted(instances.keys()):
-                actors.append(instances[window])
-            plt = show(actors,
-                       new=True,
-                       N=len(actors),
-                       sharecam=True,
-                       interactive=False,
-                       title='SofaVedo',
-                       axes=4)
-            plt.addButton(plt.interactor.TerminateApp, states=["start"])
-            plt.interactive()
-            # Once the user closed the window, recreate a new Plotter
-            camera = {'pos': plt.camera.GetPosition(),
-                      'focalPoint': plt.camera.GetFocalPoint()}
-            self.__plotter = show(actors,
-                                  new=True,
-                                  N=len(actors),
-                                  sharecam=True,
-                                  interactive=False,
-                                  title='SofaVedo',
-                                  axes=plt.axes,
-                                  camera=camera)
-
-    def update_instance(self,
-                        table_name: str,
-                        data_dict: Dict[str, Any]):
-        """
-        Update an Actor instance with updated data.
-
-        :param table_name: Name of the Table (one Table per Actor).
-        :param data_dict: Updated data of the Actor.
-        """
-
-        if len(data_dict.keys()) > 1:
-            # Sort data
-            cmap_dict = {'scalar_field': data_dict.pop('scalar_field')} if 'scalar_field' in data_dict else {}
-            # Get Actor instance
-            _, factory_id, actor_id = table_name.split('_')
-            factory_id, actor_id = int(factory_id), int(actor_id)
-            actor = self.__all_actors[(factory_id, actor_id)]
-            # If Actor cannot be updated, remove from Plotter
-            if actor.actor_type in ['Arrows', 'Markers', 'Symbols'] and not self.__offscreen:
-                self.__plotter.remove(actor.instance, at=actor.at)
-            # Update (or re-create) Actor, apply cmap
-            actor.update(data_dict).apply_cmap(cmap_dict)
-            # If Actor was re-created, add it to Plotter
-            if actor.actor_type in ['Arrows', 'Markers', 'Symbols'] and not self.__offscreen:
-                self.__plotter.add(actor.instance, at=actor.at)
-
-    def render(self):
-        """
-        Render the current state of Actors in the Plotter.
-        """
-
-        self.step += 1
-        self.__database.add_data(table_name='Sync',
-                                 data={'step': 'V'})
-
-    def __sync_visualizer(self, table_name, data_dict):
-
-        # 0. Call to render from Factory
-        if data_dict['step'] == 'F':
-            self.step += 1
-
-        # 1. Retrieve visual data and update Actors (one Table per Actor)
-        table_names = self.__database.get_tables()
-        table_names.remove('Sync')
-        for table_name in table_names:
-            # Get the current step line in the Table
-            data_dict = self.__database.get_line(table_name=table_name,
-                                                 line_id=self.step)
-            # If the id of line is correct, the Actor was updated
-            if data_dict.pop('id') == self.step:
-                self.update_instance(table_name=table_name,
-                                     data_dict=data_dict)
-            # Otherwise, the actor was not updated, then add an empty line
+        idx_factory, step = copy(self.__step)
+
+        # 1. If the group ID changed, change the visibility of Actors
+        if self.__group_change:
+            self.__group_change = False
+            # Remove previous group
+            for table_name in self.objects[self.__previous_group].keys():
+                v_object: Open3dObject = self.get_object(table_name)
+                if v_object.type == 'Text':
+                    v_object.instance.visible = False
+                else:
+                    self._scene.scene.remove_geometry(v_object.name)
+            # Add new group
+            for table_name in self.objects[self.__current_group].keys():
+                v_object = self.get_object(table_name)
+                if v_object.type == 'Text':
+                    v_object.instance.visible = True
+                else:
+                    self._scene.scene.add_geometry(v_object.name, v_object.instance, v_object.material)
+
+        # 2. Update all the Actors
+        self.update_objects(step=step,
+                            idx_factory=idx_factory)
+        self.clients[idx_factory].send(b'done')
+
+    def update_object_backend(self,
+                              v_object: Open3dObject) -> None:
+        """
+        Specific Actor update instructions.
+
+        :param v_object: Actor object.
+        """
+
+        v_object.update()
+        if v_object.group == self.__current_group:
+            if v_object.type == 'Text':
+                pass
             else:
-                self.__database.add_data(table_name=table_name,
-                                         data={})
+                self._scene.scene.remove_geometry(v_object.name)
+                self._scene.scene.add_geometry(v_object.name, v_object.instance, v_object.material)
+
+    def exit(self,
+             force_quit: bool = True) -> None:
+        """
+        Exit procedure of the Visualizer.
+
+        :param force_quit: True if the Window was manually closed.
+        """
+
+        if force_quit:
+            for i, client in enumerate(self.clients):
+                client.send(b'exit')
+                self.is_done[i] = True
+
+        # Close the socket
+        if self.server is not None:
+            self.server.close()
+            self.server = None
+
+    def _change_group(self,
+                      index: int) -> None:
 
-        # 2. Render Plotter if offscreen is False
-        if not self.__offscreen:
-            self.__plotter.render()
+        if index != self.__current_group:
+            self.__previous_group = self.__current_group
+            self.__current_group = index
+            self.__group_change = True
```

### Comparing `SimulationSimpleDatabase-22.6.2/src/Core/Storage/AdaptiveTable.py` & `SimulationSimpleDatabase-24.1/src/Core/Storage/adaptive_table.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Dict, Type, Any, Union, List, Optional
 from peewee import IntegerField, FloatField, TextField, BooleanField, BlobField, DateTimeField, ForeignKeyField, Field
 from peewee import chunked
 from playhouse.signals import Model, pre_save, post_save
 from playhouse.migrate import migrate, SqliteMigrator, SqliteDatabase
+from numpy import ndarray
 from datetime import datetime
 
-from SSD.Core.Storage.ExtendedFields import NumpyField, ndarray
+from SSD.Core.Storage.numpy_field import NumpyField
 
 
 class AdaptiveTable(Model):
     role: str = 'Adaptive'
     table_type: Dict[Type, Field] = {int: IntegerField,
                                      float: FloatField,
                                      str: TextField,
@@ -28,31 +29,29 @@
 
     @classmethod
     def database(cls) -> SqliteDatabase:
 
         return cls._meta.database
 
     @classmethod
-    def fields(cls,
-               only_names: bool = True) -> Union[List[str], Dict[str, Field]]:
+    def fields(cls, only_names: bool = True) -> Union[List[str], Dict[str, Field]]:
 
         return list(cls._meta.fields.keys()) if only_names else cls._meta.fields
 
     @classmethod
-    def connect(cls,
-                database: SqliteDatabase):
+    def connect(cls, database: SqliteDatabase) -> None:
 
         cls.bind(database)
         cls.database().create_tables([cls])
 
     @classmethod
     def extend(cls,
                field_name: str,
                data_type: Type,
-               default_value: Any):
+               default_value: Any) -> None:
 
         migrator = SqliteMigrator(cls.database())
         atts = {'null': True}
         if default_value != '_null_':
             if type(default_value) != data_type:
                 raise TypeError(
                     f"The default value type for field {field_name} of table {cls._meta.name} must be {data_type},"
@@ -63,42 +62,42 @@
         field = cls.table_type.get(data_type, BlobField)(**atts)
         migrate(migrator.add_column(cls._meta.name, field_name, field))
         cls._meta.add_field(field_name, field)
 
     @classmethod
     def extend_fk(cls,
                   model: Model,
-                  field_name: str):
+                  field_name: str) -> None:
 
         migrator = SqliteMigrator(cls.database())
         field = ForeignKeyField(model=model, backref=field_name, null=True, field=model._meta.primary_key)
         migrate(migrator.add_column(cls._meta.name, field_name, field))
         cls._meta.add_field(field_name, field)
 
     @classmethod
     def rename_table(cls,
                      old_table_name: str,
-                     new_table_name: str):
+                     new_table_name: str) -> None:
 
         migrator = SqliteMigrator(cls.database())
         migrate(migrator.rename_table(old_table_name, new_table_name))
 
     @classmethod
     def rename_field(cls,
                      old_field_name: str,
-                     new_field_name: str):
+                     new_field_name: str) -> None:
 
         migrator = SqliteMigrator(cls.database())
         migrate(migrator.rename_column(cls._meta.name, old_field_name, new_field_name))
         cls._meta.add_field(new_field_name, getattr(cls, old_field_name))
         cls._meta.remove_field(old_field_name)
 
     @classmethod
     def remove_field(cls,
-                     field_name: str):
+                     field_name: str) -> None:
 
         migrator = SqliteMigrator(cls.database())
         migrate(migrator.drop_column(cls._meta.name, field_name))
         cls._meta.remove_field(field_name)
 
     @classmethod
     def description(cls,
@@ -118,61 +117,64 @@
             desc += f' (default)\n' if field.name in ['id', '_dt_'] else '\n'
         return desc
 
     @classmethod
     def add_data(cls,
                  fields_names: List[str],
                  fields_values: List[Any],
-                 batched: bool = False):
+                 batched: bool = False) -> Union[int, List[int]]:
 
         pass
 
 
 class StoringTable(AdaptiveTable):
     role: str = 'Storing'
 
     @classmethod
     def add_data(cls,
                  fields_names: List[str],
                  fields_values: List[Any],
-                 batched: bool = False):
+                 batched: bool = False) -> Union[int, List[int]]:
 
         if not batched:
             line = cls(**dict(zip(fields_names, fields_values)))
             line.save()
             return line.id
 
         else:
             fields = [getattr(cls, field) for field in fields_names]
             batch = [tuple(samples) for samples in zip(*fields_values)]
             n = cls.select().count()
             with cls.database().atomic():
                 for chunk in chunked(batch, 100):
                     cls.insert_many(chunk, fields=fields).execute()
             N = cls.select().count()
-            return [cls.get_by_id(i + 1) for i in range(n, N)]
+            return [cls.get_by_id(i + 1).id for i in range(n, N)]
 
 
 class ExchangeTable(AdaptiveTable):
     role: str = 'Exchange'
 
     @classmethod
     def add_data(cls,
                  fields_names: List[str],
                  fields_values: List[Any],
-                 batched: bool = False):
+                 batched: bool = False) -> Union[int, List[int]]:
 
         if not batched:
             cls.delete().execute()
             line = cls(**dict(zip(fields_names, fields_values)))
             line.save()
-            return line
+            return line.id
 
         else:
             fields = [getattr(cls, field) for field in fields_names]
             batch = [tuple(samples) for samples in zip(*fields_values)]
             cls.delete().execute()
             pre_save.send(cls, created=False)
+            n = cls.select().count()
             with cls.database().atomic():
                 for chunk in chunked(batch, 100):
                     cls.insert_many(chunk, fields=fields).execute()
+            N = cls.select().count()
             post_save.send(cls, created=False)
+            return [cls.get_by_id(i + 1).id for i in range(n, N)]
```

### Comparing `SimulationSimpleDatabase-22.6.2/src/Core/Storage/Database.py` & `SimulationSimpleDatabase-24.1/src/Core/Storage/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import Union, List, Type, Dict, Tuple, Optional, Any, Callable
 from os import remove, mkdir
 from os.path import exists, join, sep, getsize
+from inspect import getmembers
+from peewee import ForeignKeyField
 from playhouse.migrate import SqliteDatabase
 from playhouse.signals import Signal, pre_save, post_save
 from datetime import datetime
 from numpy import unique
 
-from SSD.Core.Storage.AdaptiveTable import AdaptiveTable, StoringTable, ExchangeTable, ForeignKeyField
-from SSD.Core.Storage.ExtendedPeewee import generate_models
-from SSD.Core.Storage.Exporter import Exporter, ExporterJson, ExporterCSV
+from SSD.Core.Storage.adaptive_table import AdaptiveTable, StoringTable, ExchangeTable
+from SSD.Core.Storage.peewee_extension import generate_models
+from SSD.Core.Storage.exporter import Exporter
 
 FieldType = Union[Tuple[str, Type], Tuple[str, Type, Any], Tuple[str, str]]
 
 
 class Database:
 
     def __init__(self,
@@ -31,29 +33,26 @@
 
         self.__database_dir = database_dir
         self.__database_name = database_name
         self.__database: Optional[SqliteDatabase] = None
         self.__tables: Dict[str, type(AdaptiveTable)] = {}
         self.__fk: Dict[str, Dict[str, str]] = {}
         self.__signals: List[Tuple[str, Signal, str, Callable, str]] = []
-        self.__exporters: Dict[str, Tuple[Type[Exporter], str]] = {'json': (ExporterJson, 'json'),
-                                                                   'csv': (ExporterCSV, 'csv')}
 
     @staticmethod
-    def make_name(table_name: str):
+    def make_name(table_name: str) -> str:
         """
         Harmonize the Table names.
 
         :param table_name: Name of the Table.
         """
 
         return table_name[0] + table_name[1:].lower() if len(table_name) > 1 else table_name
 
-    def new(self,
-            remove_existing: bool = False):
+    def new(self, remove_existing: bool = False) -> 'Database':
         """
         Create a new Database file.
 
         :param remove_existing: If True, Database file will be overwritten.
         """
 
         # Create directory if not exists
@@ -72,16 +71,15 @@
                     index += 1
                 self.__database_name = f'{self.__database_name}({index})'
 
         # Create the Database
         self.__database = SqliteDatabase(database_path)
         return self
 
-    def load(self,
-             show_architecture: bool = False):
+    def load(self, show_architecture: bool = False) -> 'Database':
         """
         Load an existing Database file.
 
         :param show_architecture: If True, the loaded models will be printed.
         """
 
         # Check file existence
@@ -113,15 +111,15 @@
 
         # Show resulting architecture
         if show_architecture:
             self.print_architecture()
 
         return self
 
-    def get_path(self):
+    def get_path(self) -> Tuple[str, str]:
         """
         Access the Database file path.
         """
 
         return self.__database_dir, self.__database_name
 
     def print_architecture(self):
@@ -251,14 +249,19 @@
             # Add each Field to the Table
             for field in fields:
 
                 # Define name, type and default value
                 field_name, field_type = field[0], field[1]
                 field_default = '_null_' if len(field) == 2 else field[2]
 
+                # As peewee.Model creates a new attribute named field_name, check that this attribute does not exist
+                if field_name in [m[0] for m in getmembers(table)]:
+                    raise ValueError(f"Tried to create a field '{field_name}' in the Table '{table_name}'. "
+                                     f"You are not allowed to create a field with this name, please rename it.")
+
                 # Extend the Table
                 if field_name not in table.fields():
                     # FK
                     if type(field_type) == str:
                         if (fk_table_name := self.make_name(field_type)) not in self.__tables.keys():
                             raise ValueError(f"Cannot create the ForeignKey '{fk_table_name}' since this Table does not"
                                              f"exists. Created Tables so far: {self.__tables.keys()}")
@@ -327,55 +330,56 @@
                                      name=name)
         self.__signals = []
 
     def add_data(self,
                  table_name: str,
                  data: Dict[str, Any]):
         """
-        Execute a line insert query.
+        Execute a line insert query. Return the index of the new line in the Table.
 
         :param table_name: Name of the Table.
         :param data: New line of the Table.
         """
 
         table_name = self.make_name(table_name)
         return self.__add_data(table_name=table_name,
                                data=data)
 
     def add_batch(self,
                   table_name: str,
                   batch: Dict[str, List[Any]]):
         """
-        Execute a batch insert query.
+        Execute a batch insert query. Return the indices of the new lines in the Table.
 
         :param table_name: Name of the Table.
         :param batch: New lines of the Table.
         """
 
         table_name = self.make_name(table_name)
         # Check that the batch is well-formed
-        batch_values = [batch[key] for key in set(batch.keys()) - set(self.__fk[table_name])]
-        if len(unique(samples := [len(b) for b in batch_values])) != 1:
-            raise ValueError(f"The number of samples per batch must be the same for all fields. Number of samples "
-                             f"received per field: {dict(zip(batch.keys(), samples))}")
-        self.__add_data(table_name=table_name,
-                        data=batch,
-                        batched=True)
+        if table_name in self.__fk:
+            batch_values = [batch[key] for key in set(batch.keys()) - set(self.__fk[table_name])]
+            if len(unique(samples := [len(b) for b in batch_values])) != 1:
+                raise ValueError(f"The number of samples per batch must be the same for all fields. Number of samples "
+                                 f"received per field: {dict(zip(batch.keys(), samples))}")
+        return self.__add_data(table_name=table_name,
+                               data=batch,
+                               batched=True)
 
     def __add_data(self,
                    table_name: str,
                    data: Union[Dict[str, Any], Dict[str, List[Any]]],
                    batched: Optional[bool] = False):
 
         # Unpack kwargs
         fields_names = list(data.keys())
         fields_values = list(data.values())
         fields_types = []
         for name, value in zip(fields_names, fields_values):
-            if name in self.__fk[table_name]:
+            if table_name in self.__fk and name in self.__fk[table_name]:
                 fields_types.append(self.__fk[table_name][name])
             elif batched:
                 fields_types.append(type(value[0]))
             else:
                 fields_types.append(type(value))
 
         # Check table existence
@@ -567,16 +571,16 @@
                         fields_selection += (table.fields(only_names=False)[field_name],)
 
         # Define the indices of lines to select
         if lines_id is None:
             if lines_range is not None and len(lines_range) != 2:
                 raise ValueError("The range of lines must contains the first and the last line indices.")
             nb_line = self.nb_lines(table_name=table_name)
-            first_line_id = 1 if lines_range is None else lines_range[0]
-            last_line_id = nb_line if lines_range is None else lines_range[1]
+            first_line_id = lines_range[0] if lines_range is not None else 1
+            last_line_id = lines_range[1] if lines_range is not None else nb_line
             _slice = [first_line_id, last_line_id]
             for i, idx in enumerate(_slice):
                 if idx < 0:
                     _slice[i] += nb_line + 1
                 elif idx > nb_line:
                     _slice[i] = nb_line
             _slice[1] = _slice[0] + 1 if _slice[1] < _slice[0] else _slice[1] + 1
@@ -645,16 +649,16 @@
         """
         Close the Database.
 
         :param erase_file: If True, the Database file will be erased.
         """
 
         self.__database.close()
-        if erase_file:
-            remove(join(self.__database_dir, f'{self.__database_name}.db'))
+        if erase_file and exists(database_path := join(self.__database_dir, f'{self.__database_name}.db')):
+            remove(database_path)
 
     def rename_table(self,
                      table_name: str,
                      new_table_name: str):
         """
         Rename a Table of the Database.
 
@@ -733,40 +737,44 @@
 
         # Renaming
         self.__tables[table_name].remove_field(field_name)
 
     def export(self,
                exporter: str,
                filename: str,
-               tables: Optional[Union[str, List[str]]] = None):
+               tables: Optional[Union[str, List[str]]] = None) -> None:
+        """
+        Export the Database to a CSV or JSON file.
+
+        :param exporter: Exporter type ('json' or 'csv').
+        :param filename: Exported filename.
+        :param tables: Tables to export.
+        """
 
         # Check exporter format
         exporter = exporter.lower()
-        if exporter not in self.__exporters:
-            raise ValueError(f"Unknown exporter with name {exporter}. "
-                             f"Available exporters are {self.__exporters.keys()}.")
+        if exporter not in ['json', 'csv']:
+            raise ValueError(f"Unknown exporter with name {exporter}. Available exporters are ['json', 'csv'].")
 
         # Set good file extension
         file_path = filename.split(sep)
         file_name = file_path.pop(-1)
         file_name = file_name if len(file_name.split('.')) == 1 else file_name.split('.')[0]
         filename = join(*file_path[:-1], file_name)
-        extension = self.__exporters[exporter][1]
 
         # Get the tables to export
         tables = self.get_tables() if tables is None else tables
         tables = [tables] if type(tables) != list else tables
         for table in tables:
             if table not in self.get_tables():
                 raise ValueError(f"The following Table does not exist: {table}")
 
         # Export each table
         # Todo: see 'at once' version
         for table in tables:
-            _filename = filename + f'_{table}.{extension}'
+            _filename = filename + f'_{table}.{exporter}'
             if exporter == 'json':
-                query = self.get_lines(table_name=table,
-                                       batched=True)
+                query = self.get_lines(table_name=table, batched=True)
+                Exporter.export_json(filename=_filename, query=query)
             else:
                 query = self.__tables[table].select().tuples()
-            self.__exporters[exporter][0].export(filename=_filename,
-                                                 query=query)
+                Exporter.export_csv(filename=_filename, query=query)
```

### Comparing `SimulationSimpleDatabase-22.6.2/src/Core/Storage/Exporter.py` & `SimulationSimpleDatabase-24.1/src/Core/Storage/exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,51 +2,36 @@
 import json
 import csv
 from peewee import Query
 from datetime import datetime
 from numpy import ndarray
 
 
-class Exporter:
-
-    @classmethod
-    def export(cls,
-               filename: str,
-               query: Union[Dict[str, Any], Query]):
-
-        pass
-
+def default_format(o: Any):
+    if isinstance(o, datetime):
+        return o.isoformat()
+    elif isinstance(o, ndarray):
+        return o.tolist()
 
-class ExporterJson(Exporter):
 
-    @staticmethod
-    def default(o: Any):
-
-        if isinstance(o, datetime):
-            return o.isoformat()
-
-        elif isinstance(o, ndarray):
-            return o.tolist()
+class Exporter:
 
     @classmethod
-    def export(cls,
-               filename: str,
-               query: Union[Dict[str, Any], Query]):
+    def export_json(cls,
+                    filename: str,
+                    query: Union[Dict[str, Any], Query]):
 
         file = open(filename, 'w')
-        json.dump(query, file, default=cls.default)
+        json.dump(query, file, default=default_format)
         file.close()
 
-
-class ExporterCSV(Exporter):
-
     @classmethod
-    def export(cls,
-               filename: str,
-               query: Union[Dict[str, Any], Query]):
+    def export_csv(cls,
+                   filename: str,
+                   query: Union[Dict[str, Any], Query]):
 
         with open(filename, 'w') as file:
             writer = csv.writer(file)
             t = query.execute()
             t.initialize()
             if getattr(t, 'columns', None):
                 writer.writerow([column for column in t.columns])
```

### Comparing `SimulationSimpleDatabase-22.6.2/src/Core/Storage/ExtendedPeewee.py` & `SimulationSimpleDatabase-24.1/src/Core/Storage/peewee_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 from peewee import IntegerField, ForeignKeyField, BareField, CompositeKey, AutoField, DeferredForeignKey, SQL
 from playhouse.reflection import Introspector, SqliteDatabase, SqliteMetadata, UnknownField
 import warnings
 
-from SSD.Core.Storage.AdaptiveTable import StoringTable, ExchangeTable
-from SSD.Core.Storage.ExtendedFields import NumpyField
+from SSD.Core.Storage.adaptive_table import StoringTable, ExchangeTable
+from SSD.Core.Storage.numpy_field import NumpyField
 
 
 def generate_models(database, schema=None, **options):
-    # Use extended inspector
-    introspector = _ExtendedIntrospector.from_database(database, schema=schema)
+
+    # EXTENSION: Use extended inspector
+    introspector = ExtendedIntrospector.from_database(database, schema=schema)
     return introspector.generate_models(**options)
 
 
-class _ExtendedSqliteMetadata(SqliteMetadata):
+class ExtendedSqliteMetadata(SqliteMetadata):
 
     def __init__(self, database):
         super().__init__(database)
-        # Extend the columns mapper
+        # EXTENSION: Extend the columns mapper with the new NumpyField
         self.column_map['numpy'] = NumpyField
 
 
-class _ExtendedIntrospector(Introspector):
+class ExtendedIntrospector(Introspector):
 
     @classmethod
     def from_database(cls, database, schema=None):
         if isinstance(database, SqliteDatabase):
-            # Use extended metadata class
-            metadata = _ExtendedSqliteMetadata(database)
+            # EXTENSION: Use extended metadata class
+            metadata = ExtendedSqliteMetadata(database)
             return cls(metadata, schema=schema)
         return Introspector.from_database(database, schema)
 
-    def generate_models(self, skip_invalid=False, table_names=None,
-                        literal_column_names=False, bare_fields=False,
+    def generate_models(self, skip_invalid=False, table_names=None, literal_column_names=False, bare_fields=False,
                         include_views=False):
 
-        database = self.introspect(table_names, literal_column_names,
-                                   include_views)
+        database = self.introspect(table_names, literal_column_names, include_views)
         models = {}
         pending = set()
 
         def _create_model(table, models):
-
             pending.add(table)
             for foreign_key in database.foreign_keys[table]:
                 dest = foreign_key.dest_table
 
                 if dest not in models and dest != table:
                     if dest in pending:
                         warnings.warn('Possible reference cycle found between '
@@ -64,15 +62,19 @@
             class Meta:
                 indexes = multi_column_indexes
                 table_name = table
 
             # Fix models with multi-column primary keys.
             composite_key = False
             if len(primary_keys) == 0:
-                primary_keys = columns.keys()
+                if 'id' not in columns:
+                    Meta.primary_key = False
+                else:
+                    primary_keys = columns.keys()
+
             if len(primary_keys) > 1:
                 Meta.primary_key = CompositeKey(*[
                     field.name for col, field in columns.items()
                     if col in primary_keys])
                 composite_key = True
 
             attrs = {'Meta': Meta}
@@ -108,22 +110,24 @@
                     # Generate a unique related name.
                     params['backref'] = '%s_%s_rel' % (table, column_name)
 
                 if column.default is not None:
                     constraint = SQL('DEFAULT %s' % column.default)
                     params['constraints'] = [constraint]
 
-                if column_name in column_indexes and not \
-                   column.is_primary_key():
-                    if column_indexes[column_name]:
-                        params['unique'] = True
-                    elif not column.is_foreign_key():
-                        params['index'] = True
+                if not column.is_primary_key():
+                    if column_name in column_indexes:
+                        if column_indexes[column_name]:
+                            params['unique'] = True
+                        elif not column.is_foreign_key():
+                            params['index'] = True
+                    else:
+                        params['index'] = False
 
-                attrs[column_name] = FieldClass(**params)
+                attrs[column.name] = FieldClass(**params)
 
             # EXTENSION: BaseModel must inherit from our adaptive models
             class BaseModel(ExchangeTable if '_dt_' in database.columns[table] else StoringTable):
                 class Meta:
                     database = self.metadata.database
                     schema = self.schema
```

### Comparing `SimulationSimpleDatabase-22.6.2/src/Core/Storage/utils.py` & `SimulationSimpleDatabase-24.1/src/Core/Storage/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from typing import List, Tuple, Union, Optional
 
-from SSD.Core.Storage.Database import Database
-from SSD.Core.Storage.AdaptiveTable import AdaptiveTable
+from SSD.Core.Storage.adaptive_table import AdaptiveTable
+from SSD.Core.Storage.database import Database
 
 
-def merge(database_names: List[str],
-          new_database_name: str = 'merged',
+def merge(database_files: List[str],
+          new_database_file: str = 'merged',
           remove_existing: bool = False):
     """
     Merge Databases in a new Database.
 
-    :param database_names: List of Databases files.
-    :param new_database_name: Name of the new Database.
+    :param database_files: List of Databases files.
+    :param new_database_file: Name of the new Database.
     :param remove_existing: If True, Database file with name 'new_database_name' will be overwritten.
     """
 
     # Load working Databases
-    databases = [Database(database_name=database_name).load() for database_name in database_names]
-    merged_database = Database(database_name=new_database_name).new(remove_existing=remove_existing)
+    databases = [Database(database_name=database_name).load() for database_name in database_files]
+    merged_database = Database(database_name=new_database_file).new(remove_existing=remove_existing)
 
     # Create Tables with their Fields
-    print("Merging the following Databases...")
+    print("\nMerging the following Databases...")
     table_type = AdaptiveTable.table_type
     for db in databases:
         db.print_architecture()
         tables = db.get_tables()
         for table in tables:
             merged_database.create_table(table_name=table)
             for field_name, field in db.get_fields(table, only_names=False).items():
@@ -53,133 +53,142 @@
                 merged_database.add_data(table_name=table_name,
                                          data=data)
         db.close()
     merged_database.close()
     print("Merge complete.")
 
 
-def rename_tables(database_name: str,
+def rename_tables(database_file: str,
                   renamed_tables: Union[Tuple[str, str], List[Tuple[str, str]]]):
     """
     Rename Tables of the Database.
 
-    :param database_name: Database filename.
+    :param database_file: Database filename.
     :param renamed_tables: Tuple or list of tuples defined as ('old_name', 'new_name').
     """
 
     # Load the Database
-    db = Database(database_name=database_name).load()
+    db = Database(database_name=database_file).load()
 
     # Check the table names to change
     renamed_tables = [renamed_tables] if type(renamed_tables) != list else renamed_tables
     current_tables = db.get_tables()
     for (old_table_name, new_table_name) in renamed_tables:
         if old_table_name not in current_tables:
             raise ValueError(f"The Database does not contain a Table with name '{old_table_name}. "
                              f"Available Tables are {current_tables}.")
 
     # Renaming
-    print("Proceeding...")
+    print("\nRenaming Table(s). \nProceeding...")
     for (old_table_name, new_table_name) in renamed_tables:
         db.rename_table(table_name=old_table_name,
                         new_table_name=new_table_name)
     db.print_architecture()
+    db.close()
     print("Renaming done.")
 
 
-def rename_fields(database_name: str,
+def rename_fields(database_file: str,
                   table_name: str,
                   renamed_fields: Union[Tuple[str, str], List[Tuple[str, str]]]):
     """
     Rename Fields of a Table of the Database.
 
-    :param database_name: Database filename.
+    :param database_file: Database filename.
     :param table_name: Name of the Table.
     :param renamed_fields: Tuple or list of tuples defined as ('old_name', 'new_name').
     """
 
     # Load the Database
-    db = Database(database_name=database_name).load()
+    db = Database(database_name=database_file).load()
 
     # Check the fields to change
     renamed_fields = [renamed_fields] if type(renamed_fields) != list else renamed_fields
     current_fields = db.get_fields(table_name=table_name)
     for (old_field_name, new_field_name) in renamed_fields:
         if old_field_name in ['id', '_dt_']:
             raise ValueError("The following fields cannot be renamed: 'id', '_dt_'")
         elif old_field_name not in current_fields:
             raise ValueError(f"The field '{old_field_name} is not in the list of available fields: {current_fields}")
 
     # Renaming
-    print("Proceeding...")
+    print("\nRenaming Field(s). \nProceeding...")
     for (old_field_name, new_field_name) in renamed_fields:
         db.rename_field(table_name=table_name,
                         field_name=old_field_name,
                         new_field_name=new_field_name)
     db.print_architecture()
+    db.close()
     print("Renaming done.")
-    print(db.get_fields('Training'))
 
 
-def remove_table(database_name: str,
+def remove_table(database_file: str,
                  table_names: Union[str, List[str]]):
     """
     Remove Tables of the Database.
 
-    :param database_name: Database filename.
+    :param database_file: Database filename.
     :param table_names: Table(s) to remove from the Database.
     """
 
     # Load the Database
-    db = Database(database_name=database_name).load()
+    db = Database(database_name=database_file).load()
     table_names = [table_names] if type(table_names) != list else table_names
 
     # Removing
-    print("Proceeding...")
+    print("\nRemoving Table(s). \nProceeding...")
     for table_name in table_names:
         db.remove_table(table_name=table_name)
     db.print_architecture()
+    db.close()
     print("Removing done.")
 
 
-def remove_field(database_name: str,
+def remove_field(database_file: str,
                  table_name: str,
                  fields: Union[str, List[str]]):
     """
     Remove Fields of a Table of the Database.
 
-    :param database_name: Database filename.
+    :param database_file: Database filename.
     :param table_name: Name of the Table.
     :param fields: Field(s) to remove from the Table.
     """
 
     # Load the Database
-    db = Database(database_name=database_name).load()
+    db = Database(database_name=database_file).load()
 
     # Check the fields to remove
     fields = [fields] if type(fields) != list else fields
     current_fields = db.get_fields(table_name=table_name)
     for field in fields:
         if field in ['id', '_dt_']:
             raise ValueError("The following fields cannot be removed: 'id', '_dt_'")
         elif field not in current_fields:
             raise ValueError(f"The field '{field} is not in the list of available fields: {current_fields}")
 
     # Removing
-    print("Proceeding...")
+    print("\nRemoving Filed(s). \nProceeding...")
     for field in fields:
         db.remove_field(table_name=table_name,
                         field_name=field)
     db.print_architecture()
     print("Removing done.")
 
 
-def export(database_name: str,
+def export(database_file: str,
            exporter: str,
-           filename: Optional[str] = None,
-           remove_existing: bool = False):
+           filename: Optional[str] = None) -> None:
+    """
+    Export the Database file to CSV or JSON formats.
+
+    :param database_file: Database filename.
+    :param exporter: Exporter type (either 'csv' or 'json').
+    :param filename: Exported filename.
+    """
 
     # Load the Database
-    db = Database(database_name=database_name).load()
+    db = Database(database_name=database_file).load()
 
+    # Export to file
     db.export(exporter=exporter,
-              filename=filename)
+              filename=filename if filename is not None else 'export')
```

### Comparing `SimulationSimpleDatabase-22.6.2/src/SOFA/Rendering/VedoFactory.py` & `SimulationSimpleDatabase-24.1/src/SOFA/Rendering/user_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,96 @@
 from typing import Optional, Dict, Tuple, Any
 from numpy import array, ndarray, tile
 import Sofa
 
-from SSD.Core.Storage.Database import Database
-from SSD.Core.Rendering.VedoFactory import VedoFactory as _VedoFactory
+from SSD.Core.Storage.database import Database
+from SSD.Core.Rendering.user_api import UserAPI as CoreUserAPI
 from SSD.SOFA.utils import error_message
 
 
-class VedoFactory(Sofa.Core.Controller):
+class UserAPI(Sofa.Core.Controller, CoreUserAPI):
 
     def __init__(self,
                  root: Sofa.Core.Node,
                  database: Optional[Database] = None,
                  database_dir: str = '',
                  database_name: Optional[str] = None,
                  remove_existing: bool = False,
+                 non_storing: bool = False,
+                 exit_on_window_close: bool = True,
                  idx_instance: int = 0,
                  *args, **kwargs):
         """
-            A Factory to manage objects to render and save in the Database.
-            User interface to create and update Vedo objects.
-            Additional callbacks to automatically get SOFA objects Data.
-
-            :param root: Root node of the sce graph.
-            :param database: Database to connect to.
-            :param database_dir: Directory which contains the Database file (used if 'database' is not defined).
-            :param database_name: Name of the Database to connect to (used if 'database' is not defined).
-            :param remove_existing: If True, overwrite a Database with the same path.
-            :param idx_instance: If several Factories must be created, specify the index of the Factory.
-            """
+        The UserAPI is a Factory used to easily create and update visual objects in the Visualizer.
+        This SOFA version brings additional callbacks to automatically get SOFA objects Data.
+
+        :param root: Root node of the sce graph.
+        :param database: Database to connect to.
+        :param database_dir: Directory which contains the Database file (used if 'database' is not defined).
+        :param database_name: Name of the Database to connect to (used if 'database' is not defined).
+        :param remove_existing: If True, overwrite a Database with the same path.
+        :param non_storing: If True, the Database will not be stored.
+        :param exit_on_window_close: If True, program will be killed if the Visualizer is closed.
+        :param idx_instance: If several Factories must be created, specify the index of the Factory.
+        """
 
         Sofa.Core.Controller.__init__(self, *args, **kwargs)
+        CoreUserAPI.__init__(self,
+                             database=database,
+                             database_dir=database_dir,
+                             database_name=database_name,
+                             remove_existing=remove_existing,
+                             non_storing=non_storing,
+                             exit_on_window_close=exit_on_window_close,
+                             idx_instance=idx_instance)
 
         # Add the Factory controller to the scene graph
         self.root: Sofa.Core.Node = root
         self.root.addChild('factory')
         self.root.factory.addObject(self)
 
-        self.__factory: _VedoFactory = _VedoFactory(database=database,
-                                                    database_dir=database_dir,
-                                                    database_name=database_name,
-                                                    remove_existing=remove_existing,
-                                                    idx_instance=idx_instance)
-        self.__updates: Dict[int, Tuple[str, Any]] = {}
+        self.__callbacks: Dict[int, Tuple[str, Any]] = {}
+
+    def onAnimateEndEvent(self, _) -> None:
+        """
+        Event called at the end of a time step.
+        """
+
+        # Execute all callbacks
+        for object_id, (object_type, object_data) in self.__callbacks.items():
+
+            if object_type == 'Mesh':
+                self.update_mesh(object_id=object_id,
+                                 positions=self.__get_position_data(position_object=object_data))
+
+            elif object_type == 'Points':
+                positions = self.__get_position_data(position_object=object_data[0])
+                positions = positions[object_data[1]] if object_data[1] is not None else positions
+                self.update_points(object_id=object_id,
+                                   positions=positions)
+
+            elif object_type == 'Arrows':
+                positions = self.__get_position_data(position_object=object_data[1])
+                positions = positions[object_data[2]] if object_data[2] is not None else positions
+                if object_data[0] == 'vec':
+                    vectors = self.__get_force_data(object_data[3])
+                else:
+                    vectors = self.__get_position_data(object_data[3]) - positions
+                vectors = vectors[object_data[4]] if object_data[4] is not None else vectors
+                if len(vectors) == 1:
+                    vectors = tile(vectors, (len(positions), 1))
+                self.update_arrows(object_id=object_id,
+                                   positions=positions,
+                                   vectors=vectors * object_data[5])
+
+            elif object_type == 'Markers':
+                self.update_markers(object_id=object_id)
+
+        # Execute rendering
+        self.render()
 
     @classmethod
     def __get_position_data(cls,
                             position_object: Sofa.Core.Base) -> ndarray:
 
         # Try to access Data field
         if (data := position_object.getData('positions')) is None:
@@ -54,17 +98,19 @@
                 positions = None
             else:
                 positions = data.value
         else:
             positions = data.value
 
         # Check value
-        if positions is None or len(positions) == 0:
-            error_message(f"The object '{position_object.getName()}' does not contain any position data or contains an "
-                          f"empty position array.")
+        if positions is None:
+            error_message(f"The object '{position_object.getName()}' does not contain any position data.")
+        elif len(positions) == 0:
+            error_message(f"The object '{position_object.getName()}' contains an empty position array.")
+
         positions = array(positions) if type(positions[0]) != ndarray else positions
         return positions[:, :3]
 
     @classmethod
     def __get_force_data(cls,
                          force_object: Sofa.Core.Base) -> ndarray:
 
@@ -74,17 +120,19 @@
                 forces = None
             else:
                 forces = data.value
         else:
             forces = data.value
 
         # Check value
-        if forces is None or len(forces) == 0:
-            error_message(f"The object '{force_object.getName()} does not contain any force data or contains an empty "
-                          f"force array.")
+        if forces is None:
+            error_message(f"The object '{force_object.getName()} does not contain any force data.")
+        elif len(forces) == 0:
+            error_message(f"The object '{force_object.getName()} contains an empty force array.")
+
         return forces
 
     @classmethod
     def __get_topology_data(cls,
                             topology_object: Sofa.Core.Base,
                             cell_type: str) -> ndarray:
 
@@ -96,59 +144,25 @@
         # Try to access Data field
         if (data := topology_object.getData(cell_type)) is None:
             cells = None
         else:
             cells = data.value
 
         # Check value
-        if cells is None or len(cells) == 0:
-            error_message(f"The object {topology_object.getName()} does not contain any topology data or contains an "
-                          f"empty topology array with cell type value '{cell_type}'.")
-        return cells
-
-    def onAnimateEndEvent(self, _):
-        """
-        At the end of a time step.
-        """
+        if cells is None:
+            error_message(f"The object {topology_object.getName()} does not contain any topology data with cell type "
+                          f"value '{cell_type}'.")
+        elif len(cells) == 0:
+            error_message(f"The object {topology_object.getName()} contains an empty topology array with cell type "
+                          f"value '{cell_type}'.")
 
-        # Execute all callbacks
-        for object_id, (object_type, object_data) in self.__updates.items():
-
-            if object_type == 'Mesh':
-                self.__factory.update_mesh(object_id=object_id,
-                                           positions=self.__get_position_data(position_object=object_data))
-
-            elif object_type == 'Points':
-                positions = self.__get_position_data(position_object=object_data[0])
-                positions = positions[object_data[1]] if object_data[1] is not None else positions
-                self.__factory.update_points(object_id=object_id,
-                                             positions=positions)
-
-            elif object_type == 'Arrows':
-                positions = self.__get_position_data(position_object=object_data[1])
-                positions = positions[object_data[2]] if object_data[2] is not None else positions
-                if object_data[0] == 'vec':
-                    vectors = self.__get_force_data(object_data[3])
-                else:
-                    vectors = self.__get_position_data(object_data[3]) - positions
-                vectors = vectors[object_data[4]] if object_data[4] is not None else vectors
-                if len(vectors) == 1:
-                    vectors = tile(vectors, (len(positions), 1))
-                self.__factory.update_arrows(object_id=object_id,
-                                             positions=positions,
-                                             vectors=vectors * object_data[5])
-
-            elif object_type == 'Markers':
-                self.__factory.update_markers(object_id=object_id)
-
-        # Execute rendering
-        self.__factory.render()
+        return cells
 
     def __get_object(self,
-                     object_path: str):
+                     object_path: str) -> Sofa.Core.Base:
 
         # Check the path
         if object_path[0] != '@' or len(object_path[1:].split('.')) == 0:
             error_message(f"You must give the absolute path to the object to record. "
                           f"The path '{object_path}' must be defined such as '@child_node.object_name'.")
 
         # Access each child node
@@ -167,45 +181,40 @@
         object_name = object_path[1:].split('.')[-1]
         if object_name not in node.objects:
             node_path = f'{self.root.getName()}{node.getPathName()}'
             error_message(f"The object '{object_name} does not belong to node '{node_path}'. "
                           f"Available objects are {[o.getName() for o in node.objects]}.")
         return node.getObject(object_name)
 
-    ########
-    # MESH #
-    ########
-
-    def add_mesh(self,
-                 position_object: str,
-                 topology_object: Optional[str] = None,
-                 cell_type: str = 'triangles',
-                 animated=True,
-                 at: int = -1,
-                 alpha: float = 1.,
-                 c: str = 'green',
-                 colormap: str = 'jet',
-                 scalar_field: ndarray = array([]),
-                 wireframe: bool = False,
-                 compute_normals: bool = True,
-                 line_width: float = 0.):
+    def add_mesh_callback(self,
+                          position_object: str,
+                          topology_object: Optional[str] = None,
+                          cell_type: str = 'triangles',
+                          animated=True,
+                          at: int = 0,
+                          alpha: float = 1.,
+                          c: str = 'green',
+                          colormap: str = 'jet',
+                          scalar_field: ndarray = array([]),
+                          wireframe: bool = False,
+                          line_width: float = -1.) -> int:
         """
-        Add a new Mesh to the Factory.
+        Add a new Mesh to the Factory with an update callback at each time step.
 
         :param position_object: Path to an object containing position and eventually topology Data.
-        :param topology_object: Path to an object containing topology Data.
+        :param topology_object: Path to an object containing topology Data. If not defined, topology data will be
+                                searched in 'position_object'.
         :param cell_type: Type of the cells ('edges', 'triangles', 'quads', 'tetrahedra', 'hexahedra').
         :param animated: If True, the object will be automatically updated at each step.
         :param at: Index of the window in which to Mesh will be rendered.
         :param alpha: Mesh opacity.
         :param c: Mesh color.
         :param colormap: Colormap scheme name.
         :param scalar_field: Scalar values used to color the Mesh regarding the colormap.
         :param wireframe: If True, the Mesh will be rendered as wireframe.
-        :param compute_normals: If True, the normals of the Mesh are pre-computed.
         :param line_width: Width of the edges of the faces.
         """
 
         # Get the objects
         position_object = self.__get_object(object_path=position_object)
         topology_object = position_object if topology_object is None \
             else self.__get_object(object_path=topology_object)
@@ -214,74 +223,44 @@
         cells = self.__get_topology_data(
             topology_object=position_object if topology_object is None else topology_object,
             cell_type=cell_type)
         # Get the positions
         positions = self.__get_position_data(position_object=position_object)
 
         # Add object
-        idx = self.__factory.add_mesh(positions=positions,
-                                      cells=cells,
-                                      at=at,
-                                      alpha=alpha,
-                                      c=c,
-                                      colormap=colormap,
-                                      scalar_field=scalar_field,
-                                      wireframe=wireframe,
-                                      compute_normals=compute_normals,
-                                      line_width=line_width)
+        idx = self.add_mesh(positions=positions,
+                            cells=cells,
+                            at=at,
+                            alpha=alpha,
+                            c=c,
+                            colormap=colormap,
+                            scalar_field=scalar_field,
+                            wireframe=wireframe,
+                            line_width=line_width)
 
         # Register object
         if animated:
-            self.__updates[idx] = ('Mesh', position_object)
+            self.__callbacks[idx] = ('Mesh', position_object)
         return idx
 
-    def update_mesh(self,
-                    object_id: int,
-                    positions: Optional[ndarray] = None,
-                    alpha: Optional[float] = None,
-                    c: Optional[str] = None,
-                    scalar_field: Optional[ndarray] = None,
-                    wireframe: Optional[bool] = None):
+    def add_points_callback(self,
+                            position_object: str,
+                            position_indices: Optional[ndarray] = None,
+                            animated=True,
+                            at: int = 0,
+                            alpha: float = 1.,
+                            c: str = 'green',
+                            colormap: str = 'jet',
+                            scalar_field: ndarray = array([]),
+                            point_size: int = 4) -> int:
         """
-        Update an existing Mesh in the Factory.
+        Add a new Point Cloud to the Factory with an update callback at each time step.
 
-        :param object_id: Index of the object (follows the global order of creation).
-        :param positions: Positions of the Mesh DOFs.
-        :param alpha: Mesh opacity.
-        :param c: Mesh color.
-        :param scalar_field: Scalar values used to color the Mesh regarding the colormap.
-        :param wireframe: If True, the Mesh will be rendered as wireframe.
-        """
-
-        self.__factory.update_mesh(object_id=object_id,
-                                   positions=positions,
-                                   alpha=alpha,
-                                   c=c,
-                                   scalar_field=scalar_field,
-                                   wireframe=wireframe)
-
-    ##########
-    # POINTS #
-    ##########
-
-    def add_points(self,
-                   position_object: str,
-                   position_indices: Optional[ndarray] = None,
-                   animated=True,
-                   at: int = -1,
-                   alpha: float = 1.,
-                   c: str = 'green',
-                   colormap: str = 'jet',
-                   scalar_field: ndarray = array([]),
-                   point_size: int = 4):
-        """
-        Add a new Mesh to the Factory.
-
-        :param position_object:
-        :param position_indices:
+        :param position_object: Path to an object containing position Data.
+        :param position_indices: Indices of the positions to extract. If None, all the positions are used.
         :param animated: If True, the object will be automatically updated at each step.
         :param at: Index of the window in which to Mesh will be rendered.
         :param alpha: Mesh opacity.
         :param c: Mesh color.
         :param colormap: Colormap scheme name.
         :param scalar_field: Scalar values used to color the Mesh regarding the colormap.
         :param point_size: Size of the points.
@@ -291,81 +270,57 @@
         position_object = self.__get_object(object_path=position_object)
 
         # Get the positions
         positions = self.__get_position_data(position_object=position_object)
         positions = positions[position_indices] if position_indices is not None else positions
 
         # Add object
-        idx = self.__factory.add_points(positions=positions,
-                                        at=at,
-                                        alpha=alpha,
-                                        c=c,
-                                        colormap=colormap,
-                                        scalar_field=scalar_field,
-                                        point_size=point_size)
+        idx = self.add_points(positions=positions,
+                              at=at,
+                              alpha=alpha,
+                              c=c,
+                              colormap=colormap,
+                              scalar_field=scalar_field,
+                              point_size=point_size)
 
         # Register object
         if animated:
-            self.__updates[idx] = ('Points', (position_object, position_indices))
+            self.__callbacks[idx] = ('Points', (position_object, position_indices))
         return idx
 
-    def update_points(self,
-                      object_id: int,
-                      positions: Optional[ndarray] = None,
-                      alpha: Optional[float] = None,
-                      c: Optional[str] = None,
-                      scalar_field: Optional[ndarray] = None,
-                      point_size: Optional[int] = None):
-        """
-        Update an existing Point Cloud in the Factory.
-
-        :param object_id: Index of the object (follows the global order of creation).
-        :param positions: Positions of the Point Cloud DOFs.
-        :param alpha: Point Cloud opacity.
-        :param c: Point Cloud color.
-        :param scalar_field: Scalar values used to color the Point Cloud regarding the colormap.
-        :param point_size: Size of the points.
-        """
-
-        self.__factory.update_points(object_id=object_id,
-                                     positions=positions,
-                                     alpha=alpha,
-                                     c=c,
-                                     scalar_field=scalar_field,
-                                     point_size=point_size)
-
-    ###########
-    # VECTORS #
-    ###########
-
-    def add_vectors(self,
-                    position_object: str,
-                    vector_object: Optional[str] = None,
-                    dest_object: Optional[str] = None,
-                    start_indices: Optional[ndarray] = None,
-                    end_indices: Optional[ndarray] = None,
-                    scale: float = 1.,
-                    animated: bool = True,
-                    at: int = -1,
-                    alpha: float = 1.,
-                    c: str = 'green',
-                    res: int = 12):
-        """
-        Add new Arrows to the Factory.
-
-        :param position_object:
-        :param vector_object:
-        :param dest_object:
-        :param start_indices:
-        :param end_indices:
-        :param scale:
-        :param animated:
+    def add_arrows_callback(self,
+                            position_object: str,
+                            vector_object: Optional[str] = None,
+                            dest_object: Optional[str] = None,
+                            start_indices: Optional[ndarray] = None,
+                            end_indices: Optional[ndarray] = None,
+                            scale: float = 1.,
+                            animated: bool = True,
+                            at: int = 0,
+                            alpha: float = 1.,
+                            c: str = 'green',
+                            colormap: str = 'jet',
+                            scalar_field: ndarray = array([]),
+                            res: int = 12) -> int:
+        """
+        Add new Arrows to the Factory with an update callback at each time step.
+
+        :param position_object: Path to an object containing start position Data.
+        :param vector_object: Path to an object containing vector Data. If None, vectors will be computed from
+                              'dest_object' end positions.
+        :param dest_object: Path to an object containing end position Data.
+        :param start_indices: Indices of the start positions to extract.
+        :param end_indices: Indices of the vectors or the end positions to extract.
+        :param scale: Scale factor to apply to vectors.
+        :param animated: If True, the object will be automatically updated at each step.
         :param at: Index of the window in which to Mesh will be rendered.
         :param alpha: Arrows opacity.
         :param c: Arrows color.
+        :param colormap: Colormap scheme name.
+        :param scalar_field: Scalar values used to color the Arrows regarding the colormap.
         :param res: Circular resolution of the arrows.
         """
 
         # Get the objects
         position_object = self.__get_object(object_path=position_object)
         vector_object = self.__get_object(object_path=vector_object) if vector_object is not None else None
         dest_object = self.__get_object(object_path=dest_object) if dest_object is not None else None
@@ -387,121 +342,69 @@
         if len(vectors) != 1 and len(vectors) != len(positions):
             error_message("There must be a vector per DOF.")
 
         if len(vectors) == 1:
             vectors = tile(vectors, (len(positions), 1))
 
         # Add object
-        idx = self.__factory.add_arrows(positions=positions,
-                                        vectors=vectors * scale,
-                                        at=at,
-                                        alpha=alpha,
-                                        c=c,
-                                        res=res)
+        idx = self.add_arrows(positions=positions,
+                              vectors=vectors * scale,
+                              at=at,
+                              alpha=alpha,
+                              c=c,
+                              colormap=colormap,
+                              scalar_field=scalar_field,
+                              res=res)
 
         # Register object
         if animated:
             if vector_object is not None:
-                self.__updates[idx] = ('Arrows', ('vec', position_object, start_indices, vector_object,
-                                                  end_indices, scale))
+                self.__callbacks[idx] = ('Arrows', ('vec', position_object, start_indices, vector_object,
+                                                    end_indices, scale))
             else:
-                self.__updates[idx] = ('Arrows', ('dst', position_object, start_indices, dest_object,
-                                                  end_indices, scale))
+                self.__callbacks[idx] = ('Arrows', ('dst', position_object, start_indices, dest_object,
+                                                    end_indices, scale))
         return idx
 
-    def update_arrows(self,
-                      object_id: int,
-                      positions: Optional[ndarray] = None,
-                      vectors: Optional[ndarray] = None,
-                      alpha: Optional[float] = None,
-                      c: Optional[str] = None,
-                      res: Optional[int] = None):
-        """
-        Update existing Arrows in the Factory.
-
-        :param object_id: Index of the object (follows the global order of creation).
-        :param positions: Positions of the Arrows DOFs.
-        :param vectors: Vectors of the Arrows.
-        :param alpha: Arrows opacity.
-        :param c: Arrows color.
-        :param res: Circular resolution of the arrows.
-        """
-
-        self.__factory.update_arrows(object_id=object_id,
-                                     positions=positions,
-                                     vectors=vectors,
-                                     alpha=alpha,
-                                     c=c,
-                                     res=res)
-
-    ###########
-    # MARKERS #
-    ###########
-
-    def add_markers(self,
-                    normal_to: int,
-                    indices: ndarray,
-                    animated: bool = True,
-                    at: int = -1,
-                    alpha: float = 1.,
-                    c: str = 'green',
-                    symbol: str = 'o',
-                    size: float = 0.1,
-                    filled: bool = True):
+    def add_markers_callback(self,
+                             normal_to: int,
+                             indices: ndarray,
+                             animated: bool = True,
+                             at: int = 0,
+                             alpha: float = 1.,
+                             c: str = 'green',
+                             colormap: str = 'jet',
+                             scalar_field: ndarray = array([]),
+                             symbol: str = 'o',
+                             size: float = 1.,
+                             filled: bool = True) -> int:
         """
-        Add new Markers to the Factory.
+        Add new Markers to the Factory with an update callback at each time step.
 
         :param normal_to: Index of the object that defines normals of the Markers.
         :param indices: Indices of the DOFs of the object where the Markers will be centered.
         :param animated:
         :param at: Index of the window in which to Mesh will be rendered.
         :param alpha: Markers opacity.
         :param c: Markers color.
+        :param colormap: Colormap scheme name.
+        :param scalar_field: Scalar values used to color the Markers regarding the colormap.
         :param symbol: Symbol of a Marker.
         :param size: Size of a Marker.
         :param filled: If True, the symbol is filled.
         """
 
         # Add object
-        idx = self.__factory.add_markers(normal_to=normal_to,
-                                         indices=indices,
-                                         at=at,
-                                         alpha=alpha,
-                                         c=c,
-                                         symbol=symbol,
-                                         size=size,
-                                         filled=filled)
+        idx = self.add_markers(normal_to=normal_to,
+                               indices=indices,
+                               at=at,
+                               alpha=alpha,
+                               c=c,
+                               colormap=colormap,
+                               scalar_field=scalar_field,
+                               symbol=symbol,
+                               size=size,
+                               filled=filled)
         # Register object
         if animated:
-            self.__updates[idx] = ('Markers', None)
+            self.__callbacks[idx] = ('Markers', None)
         return idx
-
-    def update_markers(self,
-                       object_id: int,
-                       normal_to: Optional[int] = None,
-                       indices: Optional[ndarray] = None,
-                       alpha: Optional[float] = None,
-                       c: Optional[str] = None,
-                       symbol: Optional[str] = None,
-                       size: Optional[float] = None,
-                       filled: Optional[bool] = None):
-        """
-        Update existing Markers in the Factory.
-
-        :param object_id: Index of the object (follows the global order of creation).
-        :param normal_to: Index of the object that defines normals of the Markers.
-        :param indices: Indices of the DOFs of the object where the Markers will be centered.
-        :param alpha: Markers opacity.
-        :param c: Markers color.
-        :param symbol: Symbol of a Marker.
-        :param size: Size of a Marker.
-        :param filled: If True, the symbol is filled.
-        """
-
-        self.__factory.update_markers(object_id=object_id,
-                                      normal_to=normal_to,
-                                      indices=indices,
-                                      alpha=alpha,
-                                      c=c,
-                                      symbol=symbol,
-                                      size=size,
-                                      filled=filled)
```

### Comparing `SimulationSimpleDatabase-22.6.2/src/SOFA/Storage/Database.py` & `SimulationSimpleDatabase-24.1/src/SOFA/Storage/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Any, Dict, Tuple
 import Sofa
 
-from SSD.Core.Storage.Database import Database as _Database
+from SSD.Core.Storage.database import Database as CoreDatabase
 from SSD.SOFA.utils import error_message
 
 
-class Database(Sofa.Core.Controller, _Database):
+class Database(Sofa.Core.Controller, CoreDatabase):
 
     def __init__(self,
                  root: Sofa.Core.Node,
                  database_dir: str = '',
                  database_name: str = 'runSofa',
                  *args, **kwargs):
         """
@@ -19,22 +19,24 @@
 
         :param root: Root node of the scene graph.
         :param database_dir: Directory which contains the Database file.
         :param database_name: Name of the Database file.
         """
 
         Sofa.Core.Controller.__init__(self, *args, **kwargs)
-        _Database.__init__(self, database_dir, database_name)
+        CoreDatabase.__init__(self,
+                              database_dir=database_dir,
+                              database_name=database_name)
 
         # Add the Database controller to the scene graph
         self.root: Sofa.Core.Node = root
         self.root.addChild('database')
         self.root.database.addObject(self)
 
-        self.__updates: Dict[str, Dict[str, Tuple[Sofa.Core.Object, str]]] = {}
+        self.__callbacks: Dict[str, Dict[str, Tuple[Sofa.Core.Object, str]]] = {}
         self.__dirty: Dict[str, bool] = {}
         self.__path: Dict[str, Dict[str, str]] = {}
 
     def add_callback(self,
                      table_name: str,
                      field_name: str,
                      record_object: str,
@@ -85,20 +87,20 @@
 
         # Check Field existence
         if field_name not in self.get_fields(table_name=table_name):
             self.create_fields(table_name=table_name,
                                fields=(field_name, data_type))
 
         # Register the object
-        if table_name not in self.__updates:
-            self.__updates[table_name] = {}
+        if table_name not in self.__callbacks:
+            self.__callbacks[table_name] = {}
             self.__path[table_name] = {}
-        if field_name in self.__updates[table_name]:
+        if field_name in self.__callbacks[table_name]:
             error_message(f"The Field '{field_name}' in Table '{table_name}' is already associated with an object.")
-        self.__updates[table_name][field_name] = (obj, record_field)
+        self.__callbacks[table_name][field_name] = (obj, record_field)
         self.__path[table_name][field_name] = f'@root.{record_object[1:]}.{record_field}'
 
     def onAnimateBeginEvent(self, _):
         """
         At the beginning of a time step.
         """
 
@@ -107,17 +109,17 @@
 
     def onAnimateEndEvent(self, _):
         """
         At the end of a time step.
         """
 
         # Execute all callbacks
-        for table_name in self.__updates:
+        for table_name in self.__callbacks:
             data = {}
-            for field_name, (record_object, record_field) in self.__updates[table_name].items():
+            for field_name, (record_object, record_field) in self.__callbacks[table_name].items():
                 data[field_name] = record_object.getData(record_field).value
             self.add_data(table_name=table_name, data=data)
 
         # If a Table was not updated, add an empty line (keep one line per time step)
         for table_name, dirty in self.__dirty.items():
             if not dirty:
                 self.add_data(table_name, data={})
@@ -135,26 +137,26 @@
         table_name = self.make_name(table_name)
         # If the Table was already edited during the time then update it (keep one line per time step)
         if self.__dirty[table_name]:
             self.update(table_name=table_name, data=data)
         # Otherwise, create a new line
         else:
             self.__dirty[table_name] = True
-            _Database.add_data(self, table_name=table_name, data=data)
+            CoreDatabase.add_data(self, table_name=table_name, data=data)
 
     def print_architecture(self):
         """
         Print the content of the Database with Table(s), Field(s) and connected SOFA objects.
         """
 
         print(f'\nDATABASE {self.__database_name}.db')
         for name, table in self.get_tables(only_names=False).items():
             info = table.description(indent=True, name=name).split('\n')
             for i, line in enumerate(info[1:-1]):
                 field_name = line.split('-')[1].split(' ')[1]
-                if name in self.__updates:
-                    if field_name in self.__updates[name]:
+                if name in self.__callbacks:
+                    if field_name in self.__callbacks[name]:
                         info[i + 1] = line + f' --> {self.__path[name][field_name]}'
             for i in range(len(info) - 2):
                 info[i] += '\n'
             print(''.join(info))
         print('')
```

### Comparing `SimulationSimpleDatabase-22.6.2/src/SOFA/utils.py` & `SimulationSimpleDatabase-24.1/src/SOFA/utils.py`

 * *Files identical despite different names*

